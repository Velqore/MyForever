# 💕 Forever Yours — Romantic Website

<<< copilot/update-readme-new-features
A beautiful, interactive love website built with Node.js, Express, HTML, CSS & JavaScript.
=======
A beautiful, interactive love website built with pure HTML, CSS & JavaScript — **live on Koyeb**.

> **Note:** GitHub only shows this repository's source code and README. The actual live website is hosted on Koyeb (see link below).

## 🌐 Live Site

👉 **[View the live site on Koyeb](https://myforever-velqore.koyeb.app)**
>>> main

## ✨ Features
- 🧭 **Interactive onboarding panel** — 3-step welcome screen to enter your partner's name, choose a theme, and upload photos before the site begins
- 👤 **Dynamic name personalisation** — your partner's name is woven into headings, the kiss counter, floating words, and the footer throughout the whole site
- 🎨 **Gender-aware theming** — content (emoji accents, section copy, floating words) adapts based on the gender option chosen during onboarding
- 📸 **Personalised photo gallery** — upload your own photos during onboarding; they appear as a full-width photo strip and are blended into the mood gallery
- 💗 Custom heart cursor with trailing effect
- 🌸 Animated falling petals
- ⭐ Twinkling star canvas background
- 💌 Typewriter love letter
- 🃏 Flip cards — "Reasons I Love You"
- 💖 Interactive heart with kiss counter & burst animations
- 📜 Animated timeline of moments
- 💍 Promises section — five animated promise cards
- 🌹 Floating love words
- 🎭 Mood gallery with shimmer effects
- 🎵 Background music player — `love.mp3` is already bundled; click the 🎵 button to play/pause
- 📱 Fully responsive


## 🚀 Deploy on Koyeb (Node.js)

The site is served by an Express server, so deploy it as a **Node.js** service.

1. Push this repo to GitHub
2. Go to [koyeb.com](https://www.koyeb.com) → **New Service** → **GitHub**
3. Select your repo
4. Set **Builder** to `Buildpack` (auto-detects Node.js)
5. Set **Run command** to `node server.js` (or leave blank — the `start` script in `package.json` handles it)
6. Click **Deploy** 🎉

> **Note:** The server listens on `process.env.PORT` (defaults to `3000`). Koyeb sets this automatically.

## 🎵 Replace the Music
A bundled `public/love.mp3` is already wired up to the music toggle button.  
To swap it out, simply replace `public/love.mp3` with your own MP3 file (keep the same filename), or update the `<source>` tag in `index.html`:
## 🚀 Hosting

This site is deployed on [Koyeb](https://www.koyeb.com) using the Node.js/Express server in `server.js`, which serves the static files from the `public/` folder.

> **Why not GitHub Pages?** GitHub Pages only serves plain static files and cannot run Node.js. This project uses an Express server, so it needs a platform like Koyeb that supports Node.js.

## 🎵 Add Music (Optional)
In `public/index.html`, find the music toggle section and add:
```html
<audio id="love-song" loop autoplay muted>
  <source src="your-song.mp3" type="audio/mpeg">
</audio>
```

## 💝 Personalise
- **Name & photos** — use the onboarding panel when the site loads; no code changes needed
- **Gender / theme** — pick Female 🌸, Male ⚡, or Other 🌈 in the onboarding panel to switch the floating-word accents and section copy
- Replace the timeline dates with your real milestones
- Edit the flip-card messages with personal memories
- Change the love letter text (`<span id="typewriter-text">`) to your own words

---
*Made with love 💕*
