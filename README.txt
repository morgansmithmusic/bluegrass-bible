========================================================================
PROJECT NAME: Bluegrass Bible & Repertoire Management System
VERSION: 1.0.0
LAST UPDATED: 2026-08-27
========================================================================

1. OVERVIEW
------------------------------------------------------------------------
The Bluegrass Bible is a lightweight, zero-dependency web application 
designed for our band to view real-time transposable chord charts, build 
venue setlists, and keep our master repertoire synced across all members.

The application package includes:
  * index.html          - Main application interface.
  * master-library.json - Master library database containing all songs and charts.
  * README.txt          - Usage and workflow instructions.


2. PREREQUISITES & DEPENDENCIES
------------------------------------------------------------------------
* Server/Runtime: None (Pure client-side HTML5, CSS, and Vanilla JS).
* Web Browser: Any modern desktop or mobile browser (Chrome, Safari, Firefox, Edge).
* Local Access: Works offline directly in your browser.


3. QUICK START / SETUP
------------------------------------------------------------------------
Step 1: Save `index.html` and `master-library.json` into the same folder on 
        your computer or mobile device.
Step 2: Double-click `index.html` to open it in your web browser.


4. HOW TO USE THIS TOOL
------------------------------------------------------------------------
A. MANAGING SETLISTS
  * Switch/Create Setlists: Use the top setlist dropdown or click "+ New List".
  * Add Songs: Search by title in the quick-add bar, or click "+ Add to Setlist" 
    from the Master Library table.
  * Reorder Songs: Click and drag the handle icon (☰) on any setlist song.
  * Text/SMS Export: Click "Copy Text for SMS" to quickly format the active setlist 
    for group texts.

B. LIVE CHART VIEWING & TRANSPOSITION
  * Click "View Chart" on any song inside your setlist.
  * Transpose Key: Select a new key from the dropdown to transpose chords live.
  * Toggle Chords: Hide chords for lyrics-only practice.
  * Live Play Scroll: Tap the floating arrow button (↓) at the bottom-right to 
    scroll down 75% of the viewport smoothly while playing.

C. UPDATING OR ADDING SONGS (MASTER LIBRARY WORKFLOW)
  * To ensure the entire band operates from the exact same repertoire version, 
    the master library is centrally maintained.
  * Direct edits made locally in your browser will persist on your device via 
    `localStorage`, but will NOT automatically update other band members' files.
  * Requesting Updates: If you add a new song, correct a chord, or update lyrics, 
    click "Export Library JSON" and send the exported file (or the updated song data) 
    to the Band Lead / Maintainer to have it merged into the official release.


5. TROUBLESHOOTING & COMMON ISSUES
------------------------------------------------------------------------
* Issue: `master-library.json` is not loading when opening `index.html`.
  Fix:   If your browser blocks local JSON loading (`file://` protocol due to 
         CORS restrictions), run a lightweight local HTTP server (e.g., 
         `python -m http.server` in the directory) or host the folder on a local 
         network/GitHub Pages.

* Issue: My new setlists disappeared after clearing browser cache.
  Fix:   Setlists are stored in your browser's local cache. Use the export features 
         to back up key setlists or song edits if clearing browser data.


6. MAINTAINER & CONTACT
------------------------------------------------------------------------
Repertoire Maintainer: Band Lead
For master library updates, chord corrections, or new song additions, send 
your exported JSON or song text directly to the maintainer.