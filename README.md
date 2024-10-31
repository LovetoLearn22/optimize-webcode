Overview
This project is a simple HTML-based web layout that dynamically loads header and navbar components onto multiple pages. The structure allows for modularity and ease of updates, as the header.html and nav-bar.html files are each stored in separate files and loaded dynamically. This is helpful for websites where consistency in navigation and headers across multiple pages is essential.

Code Explanation
Dynamic Component Loading: JavaScript's fetch function is used in conjunction with DOMContentLoaded to asynchronously load header.html and nav-bar.html files into designated div containers in each page.

header.html is loaded into <div id="header-container">, and nav-bar.html is loaded into <div id="navbar-container">.
This approach keeps the main page’s codebase clean and avoids repeating the header and navbar code on every page, making updates easier. When header.html or nav-bar.html is modified, the changes automatically apply to all pages that include these scripts.
Error Handling: If the fetch operation fails (e.g., if the file isn’t found or there’s a network issue), the error is logged to the console for debugging purposes.

Header Component (header.html)
The header component (header.html) includes:

A link to the homepage (index.html) with the user's name displayed beside an SVG logo placeholder.
A search bar for site navigation and a navigation menu with links to essential sections, such as Home and About pages.
Navbar Component (nav-bar.html)
The navbar component (nav-bar.html) includes:

A horizontal navigation bar (<nav>) containing links to various sections of the site (e.g., Highlights, Life, Experience, Education, Skills, etc.).
Each link is styled with classes for padding and text emphasis, ensuring that the navigation items are visually aligned and accessible.
Usage
To implement this structure:

Place the JavaScript code in the HTML files where you want to load the header and navbar components.
Save header.html and nav-bar.html in the root directory (or update the paths if they’re in subdirectories).
This setup will render a consistent header and navigation bar across all pages that include these scripts.
