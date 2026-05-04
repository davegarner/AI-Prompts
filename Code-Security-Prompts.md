ROLE + AUDIT SCOPE
Act as a senior security engineer and red team specialist. Perform a comprehensive, adversarial security audit of the following codebase.
Assume the system will be deployed in a hostile environment with motivated attackers.
Analyze the system across all layers, including:
Frontend (UI, client logic, browser storage).
Backend (APIs, business logic, services).
Authentication and authorization flows.
Database interactions and storage. Infrastructure and deployment assumptions. Third party integrations and dependencies.



CORE OBJECTIVES + THREAT MODEL
Using the codebase from the previous audit scope, identify vulnerabilities across all severity levels. Detect logic flaws, not just known patterns. Surface chained attack paths. Highlight unknown or unconventional weaknesses.
Assume attacker creativity beyond standard checklists.
Build a threat model: Define possible attacker profiles (anonymous user, authenticated user, insider, API consumer). Identify entry points and trust boundaries. Map out sensitive assets (data, tokens, permissions, secrets).


AUTH + INPUT HANDLING
Now audit authentication and input handling.
Check for (but do NOT limit yourself to):
Authentication & Authorization: Broken auth, weak session management. Privilege escalation (vertical and horizontal). Insecure password reset flows. Token leakage or reuse.
Input Handling: Injection attacks (SQL, NoSQL, OS command, template injection). XSS (stored, reflected, DOM based). CSRF vulnerabilities. File upload exploits.


DATA SECURITY + API LOGIC
Next, audit data security and backend logic across the codebase:
Data Security: Sensitive data exposure. Weak encryption or misuse of cryptography.
Hardcoded secrets or keys. Insecure storage (localStorage, cookies, logs).
API & Backend Logic: Broken object level authorization (IDOR/BOLA). Mass assignment vulnerabilities. Rate limiting issues / brute force risks. Business logic abuse (race conditions, double spending, bypassing checks).


INFRASTRUCTURE + DEPENDENCIES
Now audit infrastructure configuration and third party dependencies:
Infrastructure & Configuration: Misconfigured headers (CORS, CSP, HSTS). Open ports, debug endpoints, admin panels. Environment variable leaks. Cloud/storage misconfigurations.
Dependencies & Supply Chain: Vulnerable packages. Unsafe imports or execution.
Malicious dependency risks.


ADVANCED THREATS + MINDSET
Go beyond standard checklists. Actively attempt to discover: Non obvious logic flaws unique to this system. Feature abuse scenarios. State desynchronization issues. Cache poisoning.
Replay attacks. Timing attacks. Multi step exploit chains combining low severity issues. Any behavior that "shouldn't be possible" but is.
Think like an attacker trying to break
assumptions. Attempt to bypass validations and safeguards. Manipulate edge cases and unexpected inputs. Explore how different components interact under stress.


OUTPUT FORMAT + RULES
Present your complete audit findings in this format: 1. Vulnerability Summary (total issues by severity). 2. Detailed Findings (title, severity, affected component, description, exploitation scenario, impact, recommended fix). 3. Attack Chains (show how multiple minor issues could be combined into a major exploit). 4. Secure Design Recommendations (architectural improvements and safer patterns).
Do NOT assume the code is safe. Do NOT skip analysis due to missing context, infer risks where needed. Be exhaustive and PARANOID in your review. If unsure, flag it as a potential risk and explain why.