-----------------------------------------------------
Tron 1980s Web Template Prompt
-----------------------------------------------------




-----------------------------
Prompt
-----------------------------


can you create me a new website inspired on the computer graphics of the 1980's movie Tron.  I will host this site on IIS 10 at the root (windows server 2025)   

Design Goals

Shared components for header and footer
Markdown-first editing for content-heavy pages
Terminal-style modals
Theme support for different hues
Each Page is templated and can be duplicated when additional pages are required
Navigation links can be updated easily from a central point such as the headder and footer
Compatable display on Mobile OS


Site wide
Header and Footer pages that are displayed on every page so they can be updated centrally

Each Page is templated and can be duplicated when additional pages are required
Navigation links can be updated easily from a central point in the header

Home page
Please ensure the links in the header are centered

"Type-in" intro animation on Home (auto typing with cursor) if possible include the following information:
Browser information from the headder
Time and date


News page
The news page will contain links to news stories i create in rich markdown format, when an item is clicked on it will open in terminal-esque screen modal display.
Please create some sample news pages.

Projects page
The projects page will follow the same format at the news page, please create some sample projects using the rich markdown engine.

TFL Subsite
This site will host information about London TFL services, each service on dedicated pages - Tube Status, Station Departure Boards, Bus Stop Departure Boards, Tram Departure Boards.  This will utalise my api key.  Each page should use an individual application js to keep the code tidy
Tube Status
This page will list all of the underground lines, it will also include the Elizabeth line as part of the underground network.  It will also include the status for the DLR, Overground network, and the tram network.  The lines should be displayed as a list with an expand button to display all information that is provided by the API 

Station Departure Boards
This page will include a autocomplete search function to lookup individual stations and list each platform with the departures for each line as a Card with 3 cards per line.  no more than 3 trains should be displayed by default and should include an expand button to expand the list to show more trains provided by the api, this will show all trains available within the card and can be scrolled through so not to change the size of the card.
Ensure that where there are large interchange stations such as paddington or stratford that info is provided for the stations

Bus Stop Departure Boards
This page will include a autocomplete search function to lookup individual bus stop locations Card with 3 cards per line.  no more than 3 busses should be displayed by default and should include an expand button to expand the list to show more busses provided by the api, this will show all busses available within the card and can be scrolled through so not to change the size of the card.
Ensure that information displayed is useful to an end user rather than a bus stop ID




Secure Portal
This subsite will integrate with my entra tenant to provide access to a secure site.  This site will be available when a user authenticates to entra through an app registration and provide access to internal information pages

About page
Use rich markdown for this page so that i can edit with ease.  
Display this page as a modal that doesnt go beyond the page, the modal can be scrolled.

Create 2 sub sites:
1: Tools
For each tool, use dedicated .js files for each tool so that the mail app.js file does not become too large
this site contains the following pages

password generator
This page will be used to generate passwords in the with the following requirements
3 blocks of 6 letters seperated by a hyphen
each block contains unique letters all lower case
change any of the 2 letters in the whole 3 blocks to be a number and uppercase letters
as part of the form, add fields to create username and website
create buttons to download the password and fields into a csv file


Downloads
What: Host files (pdf, zip, assets) with checksums and short notes.
Model: content/downloads/downloads.json → direct links in assets/ or external URLs.
UI: List with file size and optional SHA256; click to download (no modal needed).


Gallery (Images or ASCII)
What: Screens, posters, concept art or ASCII art.
Model: content/gallery/gallery.json → entries referencing image files or embedded ASCII in Markdown.
UI: Grid → click shows full details in modal; green tint via CSS filters.

Contact & Keys
What: A contact page with PGP public key / fingerprints, social links, and a simple contact method.
Model: content/contact.md
UI: Markdown panel (no modal necessary).

Please ensure that links to the main site also continue to work when clicked from within the tools sub site

The second site is:
2: Travel

Keep this in the same format as the tools subsite, it will contain 3 pages that we will develop later in the project.  
for now create placeholder pages for this work.



for additional settings create:
create different themes that switch the colour, offer several different colours such as a blue hue, lighter green hue, yellow hue, orange hue.
Search/filter on News/Projects
can you center the page within the browser and also allow it to work well in a mobile browser.