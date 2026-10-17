# Ruko
Run locally: `node server.js` then open http://localhost:3000 (Node 18+, no installs needed).
Deploy: put these files in a GitHub repo, then on render.com choose New > Web Service, pick the repo,
Build Command: (leave empty), Start Command: `node server.js`.
Data is stored in `data/data.json`. On Render's free plan this file is wiped on restarts/redeploys;
add a Render Disk and set the environment variable DATA_DIR to its mount path to keep it.

## Admin account
Log in with username `Ruko`. Its password is read from the ADMIN_PASSWORD environment variable
(on Render: your service > Environment > Add Environment Variable). It is not stored in the code.
The Admin tab lets Ruko rename or delete any player hat or game and change hat prices.
