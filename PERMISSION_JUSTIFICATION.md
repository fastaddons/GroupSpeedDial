## Permission justification:

- "**Hide and show browser tabs**"
  - in Firefox we use "hidden tab" to create thumbnails (also as part of the "Auto-reload" feature).

- "**Access browser tabs**"
  - allows to access URL and title of all opened tabs - this is used for "Add all opened tabs to dials" feature

- "**Access browser activity during navigation**"
  - used in "Thumbnails generation" to detect page has finished loading and to retrieve iframes inside the hidden tab
  - used in "Already opened page detection" feature (to detect page load without injecting javascript!)

- "**Access your data for all websites**"- also known as "<all_urls>" permission (allows access to all hosts), used for:
  - "Thumbnails generation" - to be able to inject javascript into the page - this javascript extracts page title, hides scrollbar and alters "zoom" level if needed to make page fit into thumbnail. The "<all_urls>" is also needed to take screenshot of the page and to remove "security headers" so that the page can load inside "iframe" (which is usually forbidden).
  - "Favicon download" - to be able to download favicon from the page (for example "https://www.google.com/favicon.ico")
  - "Live dials" - same as during the thumbnails generation, we need to remove the security headers and optionally inject script that hides scrollbars
  - "Services integration" - as part of the "<all_urls>" permission, this allows also to optionally integrate with my "cloud server" at "group-speed-dial.fastaddons.com", optional "google favicon download" service and optional "maketext.io" (service for "text thumbnail" generation) integration

## Optional permissions - used only in specific features:

- "**Read and modify bookmarks**"
  - this can be used to import bookmarks during the initial setup
- "**Download files and read and modify the browser’s download history**"
  - allows to export (download) thumbnails with a single click (asynchronous IndexedDB database export wouldn't be possible with a single click)
- "**Access recently closed tabs**"
  - for a special dial called: "Recently closed tabs", that shows recently closed tabs and windows
- "**Access browsing history**"
  - for a special dial called: "Top sites", that shows most visited sites (same as on the "about:home" or "chrome://new-tab-page" page)

