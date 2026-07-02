# iPod Classic × Spotify

A retro iPod interface for your Spotify, hosted free on GitHub Pages.

## Setup (10 minutes, all in the browser)

### 1. Put it on GitHub
1. Create a GitHub account (free) if you don't have one.
2. Click **New repository**, name it `ipod` (or anything), keep it **Public**, create it.
3. Click **uploading an existing file** and drag in all files from this folder:
   `index.html`, `manifest.json`, `icon-180.png`, `icon-512.png`
4. Commit.

### 2. Turn on GitHub Pages
1. In the repo: **Settings → Pages**
2. Source: **Deploy from a branch**, Branch: **main**, folder: **/ (root)**. Save.
3. After a minute your app is live at:
   `https://YOUR-USERNAME.github.io/ipod/`

### 3. Connect Spotify
1. Go to https://developer.spotify.com/dashboard and log in with your Spotify account.
2. **Create app**. Name: anything. Redirect URI: your exact GitHub Pages URL, e.g.
   `https://YOUR-USERNAME.github.io/ipod/`
   (must match exactly, including the trailing slash — the app's setup screen shows you the exact value to use)
3. Under **APIs used**, tick **Web API**. Save.
4. Copy the **Client ID**.
5. Open your GitHub Pages URL on your iPhone, paste the Client ID, sign in.

### 4. Make it an app
Safari → Share → **Add to Home Screen**. Done — it launches full screen with its own icon.

## Notes
- Playback control (play/pause/skip, starting songs) requires **Spotify Premium** and the Spotify app open in the background — this app acts as a remote via Spotify Connect.
- On Spotify Free you can still browse your library and see what's playing.
- To update the app later, just edit `index.html` in the repo — GitHub Pages redeploys automatically.
