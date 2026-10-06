# Friends Wishes

This is a static website. The browser loads `index.html`, and the video opens
from its hosted ScreenApp link.

## Run locally

Open `index.html` in a browser, or start a local web server from this folder:

```powershell
py -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy

Upload these files to any static web host:

```text
index.html
```

The page can be deployed using Netlify, Vercel, Cloudflare Pages, Firebase
Hosting, or any normal web server. The video is hosted separately and is
opened by the link in `index.html`.

## Important security note

The username and password are currently stored in the browser-side JavaScript,
so this login is only a visual gate and is not real security. Anyone who can
download the page can inspect the credentials. Do not use it to protect
private or sensitive content without moving authentication to a server.
