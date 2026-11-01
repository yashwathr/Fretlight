# Fretlight

**A pocket guitar that runs in your phone's browser. By Yashwath.**

Fretlight is a playable guitar built as a single HTML file with no build step or framework. Every note is generated in real time with the Web Audio API using Karplus-Strong plucked-string synthesis, so it uses no audio samples. Fretting and strumming are separate actions, as on a real guitar. You pick a chord with one hand and strum the strings with the other.

## Features

### Playing
- **Chord tiles:** 17 open and barre chords (E, Em, Em7, A, Am, D, Dsus4, G, C, F, Bm and more). Selecting a chord sets the fretting and makes no sound by itself.
- **Strum zone:** tap a string to pluck it, or swipe across the strings to strum.
- **String bend:** hold a string to bend it up a whole step and release.
- **Auto vibrato** on sustained notes, with an adjustable amount.

### Auto-strum
- Continuous strumming that keeps its rhythm through chord changes.
- **Custom strum patterns:** build your own up/down/rest pattern, or pick a preset (Folk, Pop ballad, Reggae skank, Waltz).
- **Per-string control:** toggle which strings take part in the auto-strum.
- Upstrokes catch only the top strings, so they sound different from downstrokes.

### Sound
- **4 amp models:** Acoustic, Clean Electric, Crunch and Lead.
- Controls for sustain, tone, body resonance, vibrato, reverb and volume.
- A pick-attack transient and small pitch variations on each note.
- 7 tunings (Standard, Drop D, DADGAD, Open G and more) and a capo.

### Practice tools
- **Backing beat:** synthesized drums (Rock, Folk, Ballad, Reggae) locked to the auto-strum tempo.
- **Song practice:** 16 well-known chord progressions. The app cycles through the chords with the tempo and strum pattern while you play along.
- **Metronome** with tap tempo.
- **Looper** for recording and replaying phrases.

## Tech
- Plain HTML, CSS and JavaScript in one file
- Web Audio API for all sound (Karplus-Strong synthesis, drum synthesis and effects)
- Note buffers are cached and pre-warmed, which keeps latency low on mid-range phones
- A flat, GPU-light UI with no blur filters or heavy animations
- Works offline once loaded, apart from the Google Fonts request

## Usage
Open `index.html` in a mobile browser. On Android Chrome you can use **Menu → Add to Home screen** to install it as an app. For local testing, open the file in any modern desktop browser.

## Notes
Song entries contain chord names and strum patterns only, with no lyrics or melodies.

## License
Add your preferred license here, for example MIT.
