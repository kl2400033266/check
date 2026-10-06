# Friends Wishes

This is a static website. The browser loads `index.html` and the video from
`friends-wishes.mp4` in the same folder.

## Run locally

Open `index.html` in a browser, or start a local web server from this folder:

```powershell
py -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy

Upload both files to any static web host and make sure the files stay at these
paths:

```text
index.html
friends-wishes.mp4
```

The page can be deployed using Netlify, Vercel, Cloudflare Pages, Firebase
Hosting, or any normal web server. If the host has a file-size limit, upload
`friends-wishes.mp4` to object storage or a video host and change the
`<source src="friends-wishes.mp4">` path in `index.html` to the video's public
URL.

The video is approximately 286 MB, so it is too large for several Git-based
hosting workflows. Hosting the video separately is the most portable option.

## Important security note

The username and password are currently stored in the browser-side JavaScript,
so this login is only a visual gate and is not real security. Anyone who can
download the page can inspect the credentials. Do not use it to protect
private or sensitive content without moving authentication to a server.
