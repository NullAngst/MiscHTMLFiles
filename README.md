# HTML Projects

A collection of standalone single-file HTML applications. No build tools, no dependencies to install, no server required — just open a file in a browser and it works.

---

## Projects

### 🎬 Movie Catalog (`moviesite.html`)
A personal movie collection manager that runs entirely in the browser.

- Add movies with title, format, release year, barcode/UPC, and a short review
- Search your collection by title
- Expand any entry to see full details or remove it
- Export your collection as a `.json` file and import it back on any device
- Data persists locally via `localStorage`

---

### 📚 Book Catalog (`booksite.html`)
The same concept as the Movie Catalog, built for books.

- Add books with title, author, ISBN, condition, release year, and review
- Search by title or author
- Expand any entry for full details or to remove it
- JSON import/export for portable backups
- Data persists via `localStorage`

---

### 🍌 Banana Bread (`banana_bread.html`)
An interactive recipe page for a chocolate pecan banana bread, built around a data-driven approach to moisture.

- Three-tab layout: The Process, The Science, Shopping List
- Batch size slider scales all ingredient amounts from 1 to 3 loaves
- Clickable step cards track your progress through the recipe
- Ingredients are shown inline per step so you don't have to scroll
- Chart.js charts visualize wet-to-dry ratios and banana ripeness impact

---

### 🎵 Analog Audio Restorer Pro (`WebDawPro.html`)
A browser-based audio processing tool built on the Web Audio API.

- Import any audio file from your device
- Real-time waveform monitor and spectrum analyzer
- Transport controls with variable playback speed and volume
- High-pass and low-pass filters for removing rumble and tape hiss
- 5-band parametric equalizer with a live response graph
- Bypass toggle to A/B the processed vs. dry signal
- Export the processed audio as a WAV file

---

### 💣 Minesweeper Pro (`minesweeper.html`)
A full-featured Minesweeper clone with multiple visual themes.

- Three difficulty presets (Beginner, Intermediate, Expert) plus a custom mode
- Three themes: Deep Blurple (dark), Light, and a pixel-accurate 90s classic recreation
- First-click protection — you will never hit a mine on the first click
- Flag counter, timer, and win/loss modals
- Responsive layout that works on mobile

---

### 😱 The Corridors (`horror.html`)
A first-person 3D horror maze game running in the browser via Three.js.

- Procedurally generated maze using a recursive backtracker algorithm
- Enemies that track and pursue the player
- Health system with progressive visual distortion (blur, color shift, FOV warp) as damage increases
- Synthesized audio using the Web Audio API — no external sound files
- Mouse sensitivity control in the pause menu
- Difficulty scales with depth — each level increases enemy count and speed
- Click ENTER to start, WASD to move, mouse to look, click to shoot

---

### 👻 Lost Records: Tape 3 (`brft3.html`)
A piece of fan-fiction set in the world of *Lost Records: Bloom & Rage*.

A hypothetical conclusion written from the perspective of Swann Holloway, covering what a third tape might look like. Styled to match the game's aesthetic with a VHS scanline overlay, Cinzel headings, and a violet color palette.

---

### 🗺️ The Vagabond's Dossier (`vagabond.html`)
An interactive survival guide for nomadic life in the United States.

- Sidebar navigation with 11 sections: Ethos, Day-to-Day, Travel, Weather, Transport, Shelter, Gear, Income, Needs, Emergencies, and Legal/Wildlife
- Seasonal travel dossiers covering regional hubs, food sources, water, work, legal status, and threat assessments for each time of year
- Transport comparison covering hitchhiking, train hopping, cycling, walking, and carpooling apps
- Wildlife encounter protocols presented as a quick-reference table
- Covers the legal landscape post-*Grants Pass v. Johnson* (2024)

---

### 🔴 Silent Hill: Good+ Ending Guide (`SilentHill1Good_EndingGuide.html`)
An interactive walkthrough for unlocking the best ending in *Silent Hill* (1999).

- Three-phase structure: Hospital, Resort Area, Carousel
- Click-to-reveal step cards keep the interface clean until you need detail
- Kaufmann investigation presented as a sequential flowchart
- Scroll-spy navigation highlights your current section
- Lore boxes in each phase with developer notes and real-world inspirations

---

## Usage

All files are self-contained. Download any `.html` file and open it directly in a browser. No internet connection is required for most projects (CDN fonts and libraries are the only external dependencies, and those degrade gracefully).

The catalogs (`booksite.html`, `moviesite.html`) use `localStorage` to persist data in your browser. Use the **Export to JSON** button regularly if you want a portable backup that survives a cache clear.

---

## Tech Stack

| Tool | Used In |
|---|---|
| Tailwind CSS (CDN) | All projects |
| Three.js | `horror.html` |
| Chart.js | `banana_bread.html`, `workout.html` |
| Web Audio API | `WebDawPro.html`, `horror.html` |
| Google Fonts | `banana_bread.html`, `brft3.html`, `minesweeper.html`, `vagabond.html`, `SilentHill1Good_EndingGuide.html` |
| Lucide Icons | `WebDawPro.html` |
| Font Awesome | `workout.html` |
| localStorage | `booksite.html`, `moviesite.html` |
