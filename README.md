# GES 2027 Website

A simple, responsive landing page for the Global Entrepreneurship Summit. It has a live countdown, a 3-day schedule you can filter, and speaker cards that flip to show their bios.

**Live demo:** _add your link here_

## What's inside

- **Countdown timer:** counts down to the summit start in real time. When it hits zero, it shows "The summit is live."
- **3-day schedule:** switch between Day 1, 2 and 3 using tabs. You can also filter by Keynote, Panel or Workshop. The page never reloads.
- **Speaker cards:** hover (or tap on mobile) to flip a card and see the speaker's bio and session.
- **Responsive:** works on phones, tablets and desktops. It also has a dark mode and respects "reduce motion" settings.

## Built with

Plain HTML, CSS and JavaScript. No frameworks, no build step.

## Run it

1. Download or clone this repo.
2. Open `index.html` in your browser. That's it.

## Change the content

Open the file and edit these three things at the top of the script:

- `START`: the summit start date and time
- `SPEAKERS`: names, roles and bios
- `DAYS`: the sessions for each day

## Deploy

Push to GitHub, then turn on **GitHub Pages**. You can also drag the folder into **Netlify** or import the repo in **Vercel**.

## How it works (quick notes)

- The countdown uses a fixed timezone offset (`+05:30`), so everyone sees the same time left.
- The schedule uses one `state` object (selected day and filter). Whenever it changes, the list is drawn again.
- The card flip uses CSS 3D: `perspective`, `preserve-3d` and `backface-visibility`.
