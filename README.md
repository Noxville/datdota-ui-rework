# datdota-ui-rework
Sandbox for fiddling with elements of styling and UI 

Elements
---------

* Default layout: sidebar, header, footer, main
* Main layouts: unabridged or v-split (i.e. query/result)
* Query elements: filters, buttons
* Result elements: datatables, graphs
* Generic elements: team / hero logos, team links, player links

Gotchas
--------

- Don't try edit any vendor files (but feel free to replace them with newer versions if you require).
- A bunch of static assets in the mock_stuff folder to use.
- `dev.bat` and `dev.sh` use Python 3's http.server to serve the files, 
but use whatever you'd like (i.e. node's http-server).
- There's a html injection script (cis.js) allowing easy injection of random blobs of html. 
Don't try include js in those though: keep js inside main.js, something that main.js imports, or a <script> tag (if it's local to some html and will eventually live with that html). Might split -> queries.html and datatables.html later.
