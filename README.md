### what's going on

Starting in next@13.4.3, the custom server behaves differently and serves 404s
for static assets served out of `_next/`

This custom server is is sitting inside an express app. See `server.js` for the
implementation

### how to run it

- `npm start` to run the server on port 3000
- `sh test.sh` to make a simple curl to the main app file

On next@13.4.2, this request will 200. On next@13.4.3, the request 404s.
