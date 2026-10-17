# Arjun's Birthday Surprise

A premium 10-route React birthday experience for Arjun from Aryan. The routes are:

`/`, `/story`, `/roast`, `/gallery`, `/cake`, `/quiz`, `/letter`, `/wishes`, `/surprise`, and `/finale`.

## Run locally

1. Install current Node.js (it includes npm): https://nodejs.org/
2. In this folder, run:

   ```powershell
   npm install
   npm run dev
   ```

3. Open the local address Vite prints (normally `http://localhost:5173`).

To make a production build, run `npm run build`, then `npm run preview`.

## Make it personal

- Most visible copy can be clicked and edited in the browser for a quick preview. For permanent changes, edit `src/App.tsx`.
- Replace gallery images in `public/assets/photos/`; keep the filenames or update the `photos` list near the top of `src/App.tsx`.
- The supplied optional audio is `public/assets/birthday-track.m4a`. It never autoplayes; the gold music button starts it only after a click.
- Quiz progress uses this browser's local storage. Use **Replay quiz** to reset it.
- The story, roast, letter, quiz, and surprise intentionally use editable prompts instead of invented personal details.

## Deploy on GitHub Pages

The project is already prepared for GitHub Pages. It uses hash URLs (for example `https://USERNAME.github.io/REPOSITORY/#/quiz`) so every page works on GitHub Pages without a server configuration.

1. Create a new empty GitHub repository, for example `arjun-birthday-surprise`.
2. In this folder, run the following commands after logging in to GitHub with Git:

   ```powershell
   git init
   git add .
   git commit -m "Create Arjun birthday surprise"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/arjun-birthday-surprise.git
   git push -u origin main
   ```

3. On GitHub, open the repository’s **Settings → Pages** and set **Source** to **GitHub Actions**.
4. Open the **Actions** tab. The “Deploy birthday site to GitHub Pages” workflow will build and publish the website automatically.
5. After it succeeds, share the URL shown by the workflow. It will normally be:

   `https://YOUR-USERNAME.github.io/arjun-birthday-surprise/`

Every later `git push` to `main` publishes your latest edits automatically.
