# Rekordbox Harmonic Suite & Collection Analyzer (Windows 11)

A sleek, dark-mode Pioneer DJ-inspired desktop application built to analyze Rekordbox XML collection exports, calculate harmonic mix blends, dissect diatonic chords, compare tracks side-by-side, and explore artist/label catalogs.

---

## ⚡ Quick Start on Windows 11

### Option 1: Standalone Browser Launch (Zero Installation)
1. Extract `Rekordbox_Harmonic_Suite_Win11.zip`.
2. Double-click `rekordbox_analyzer.html`.
3. It opens immediately in **Microsoft Edge**, **Google Chrome**, or your default browser.
4. Drag and drop your exported `rekordbox.xml` file directly onto the interface (or click **Load Demo Library** to test immediately).

### Option 2: One-Click Desktop Launcher
1. Double-click `run_analyzer.bat`.
2. If Python is installed, it starts a local background server and launches your browser.
3. If Python is not installed, it automatically launches `rekordbox_analyzer.html` directly in your browser.

---

## 🎧 Core Features

### 1. Rekordbox XML Parsing & Collection Statistics
- **Instant Local Parsing**: Drag-and-drop your XML collection export. Everything runs 100% client-side in your browser for privacy and speed.
- **Metric Cards**: Total tracks, unique artists, record labels, average tempo, key dominance (% minor keys), and total collection playtime.
- **Interactive BPM Distribution Spectrum**: Visual histogram categorizing your collection into tempo brackets (Halftime 60–95, House/Techno 120–132, Dubstep/Grime 136–145, Phonk 145–165, Drum & Bass 165–180).
- **Camelot Harmonic Wheel Radar**: 12-wedge radial clock mapping key density across 1A–12A (Minor) and 1B–12B (Major).

### 2. Harmonic Mixing & Blend Engine
- **Camelot & Musical Tonality Mapping**: Full support for Camelot codes (1A–12B), standard keys (e.g. Am, F#m, C), and Open Key notations.
- **Blend Categories**:
  - **Exact Match (Same Key)**: 100% harmonic union for seamless 32-bar bass swaps.
  - **Harmonic Flow (±1 Fifth)**: Natural ascending/descending key progressions.
  - **Relative Major/Minor (A/B Swap)**: Dramatic mood changes (e.g. 8A Am ↔ 8B C Major).
  - **Energy Boost (+2 Camelot / +1 Semitone)**: Peak-time tension builders and drop-swap modulations.
  - **Halftime / Double-Time Blends**: Automatically detects 2x and 0.5x tempo syncs (e.g., 70 BPM halftime into 140 BPM dubstep, or 87 BPM into 174 BPM DnB).
- **Pitch Fader Calculator**: Calculates the exact CDJ pitch fader percentage adjustment (`Δ%`) needed on Deck B to beatmatch with the selected track.

### 3. Diatonic Music Theory & Chords Breakdown
- **Musical Scale Notes**: Exact diatonic notes for each key.
- **Diatonic Triads**: Roman numeral chords and exact chord names (e.g. for 8A / A Minor: `Am`, `Bdim`, `C`, `Dm`, `Em`, `F`, `G`).
- **Diatonic 7th Chords**: Deep, lush chords for jazz and melodic bass depth (`Am7`, `Bm7b5`, `Cmaj7`, `Dm7`, `Em7`, `Fmaj7`, `G7`).
- **Signature Sub-Bass Fundamental**: Displays acoustic tuning frequencies in Hertz (Hz) for sub-bass sound system calibration (e.g. `55.0 Hz` for A1, `41.2 Hz` for E1, `43.7 Hz` for F1).
- **Common Bass Chord Progressions**: e.g., `i - VI - VII` and `i - iv - v`.

### 4. Track Differentiation & Side-by-Side Comparison
- Click **Compare** on any candidate track to open the dual-deck inspector (`Deck A` vs `Deck B`).
- Compares:
  - Exact harmonic interval & distance on the Camelot wheel.
  - Beat difference and CDJ fader adjustment (`+0.0%`).
  - Energy and emotional dynamic shift.
  - Genre and label divergence.
  - Tailored DJ transition strategy (e.g., 32-bar EQ bass swap, filter sweep, buildup drop-swap).

### 5. Artist & Label Catalog Explorer
- Click any **Artist** or **Label** badge to inspect all other tracks by that artist or label in your library.
- View track count, primary genres, release years, and jump directly to harmonic analysis.

### 6. DJ Setlist Stager & Flow Checker
- Click `+ Set` to stage tracks into a live mix queue.
- Inspect the sequential flow between consecutive tracks to catch key clashes or extreme tempo jumps before playing live.
- Export staged setlists to `.m3u` playlist format.

---

## 📁 How to Export Your Collection from Rekordbox
1. Open **Rekordbox**.
2. Go to **File > Export Collection in XML format**.
3. Save `rekordbox.xml` to your computer.
4. Drag and drop `rekordbox.xml` onto the **Rekordbox Harmonic Suite** window.
