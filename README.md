# Gallery Hours

A picture frame for the iPad: public-domain art from the Cleveland Museum of Art (with the Art Institute of Chicago as a backup), paired with your Spotify music, in two rooms — **Calm** and **Jazz Club** — with a sleep timer that fades the room to black and stops the music.

Live page: https://homeplans-crypto.github.io/gallery-hours/

## Setup

1. **GitHub Pages:** in this repo, Settings → Pages → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save. The page goes live at the address above within a minute or two.
2. **Spotify app:** at developer.spotify.com/dashboard, create an app.
   - Redirect URI: `https://homeplans-crypto.github.io/gallery-hours/`
   - APIs used: tick **Web API** and **Web Playback SDK**.
   - Copy the app's **Client ID**.
3. **iPad:** open the live page in Safari → Settings → paste the Client ID → Connect Spotify → choose a playlist for each room.
4. **iPad settings:** keep it plugged in, and set Display & Brightness → Auto-Lock to 2 minutes. The frame keeps the screen on while a room is open; Auto-Lock turns it off after the sleep timer ends.

## Notes

- Needs Spotify Premium (both for the developer app and for playback).
- Use it in Safari. A home-screen icon may not keep the Spotify login.
- iPads may ignore volume changes from web pages, so the sleep timer may stop the music instead of fading it. The screen still dims gradually.
- Nothing secret lives in this repo. The Client ID is entered on the device and stored only in that browser.
