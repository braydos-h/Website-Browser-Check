# website-os-checker

This project contains a single HTML page that lists device information that your browser can access. Open `index.html` in a modern browser and it will display details such as:

- User agent and platform
- Available languages
- CPU count and memory (if available)
- Screen resolution and color depth
- Network connection information
- Time zone
- Optional geolocation and media devices (may prompt for permission)

## Viewing locally

For full functionality, serve `index.html` over HTTP instead of opening it
directly from the filesystem. Many browsers restrict access to geolocation and
media devices when a page is loaded as a local file. A quick way to serve the
page is with Python's built‑in HTTP server:

```bash
python3 -m http.server
```

Then navigate to `http://localhost:8000/index.html`.

The application runs entirely in the browser — no server-side code is involved.
