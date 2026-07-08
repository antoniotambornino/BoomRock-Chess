[BoomRockChess_README.md](https://github.com/user-attachments/files/29783785/BoomRockChess_README.md)
# BoomRock Chess

**By Antonio Modest Tambornino**

---

## What It Is

BoomRock Chess is a full-featured chess game with a comic-book visual identity. It runs in a single self-contained HTML file and is installable as a Progressive Web App on any phone, tablet, or desktop. No account, no server, no install required to play locally — just open the file.

Features include a built-in chess clock with increment, move highlighting, legal move enforcement, board flip, and an integrated help system.

---

## Features

**Chess Engine**
- Full legal move generation for all piece types including en passant, castling (kingside and queenside), and pawn promotion
- Illegal move prevention — only valid squares highlight for selection
- Check, checkmate, and stalemate detection

**Chess Clock**
- Built-in timer with configurable time control and increment
- Increment is added to the player who just moved
- Multiple presets: Bullet, Blitz, Rapid, Classical
- Clock pauses automatically when a player is in check

**Board Controls**
- Click or tap to select a piece — legal target squares illuminate
- Tap a highlighted square to move
- *Flip Board* button swaps perspective for over-the-board play
- Move hint system shows available moves for the selected piece

**Lawrence Square**
- A special annotated square on the board honours Lawrence Erasmus Peregrine and the Linnean Society — hover or tap the square to see the reference and link

**Visual Design**
- Comic-book title logo using the *Bangers* display font with speed-line backdrop and letterpress shadow
- Dark navy/indigo palette (`#1a1a2e`) with gold piece accents
- Responsive layout — works at any screen size

**Multiplayer (local or networked)**
- Pass-and-play on one screen out of the box
- WebSocket multiplayer is available if the file is hosted on a server that supports it

**Music Integration**
- Classical chess music playlist via YouTube Music

---

## Time Control Presets

| Name | Time | Increment |
|------|------|-----------|
| Bullet | 1 min | 0 sec |
| Blitz | 3 min | 2 sec |
| Rapid | 10 min | 0 sec |
| Classical | 30 min | 30 sec |

Time and increment are configurable in the time control panel below the board.

---

## Installation (PWA)

BoomRock Chess is installable as a Progressive Web App:

- **Android (Chrome)**: open the file → tap the *Install* banner at the bottom of the screen, or tap the browser menu → *Add to Home Screen*
- **iOS (Safari)**: tap the Share button (⎙) → *Add to Home Screen*
- **Desktop (Chrome / Edge)**: click the install icon in the address bar

Once installed, the app runs offline with a full-screen native experience and its own icon.

**Electron desktop app**: the repository also includes a `BoomRockChess-App.zip` containing an Electron wrapper for distribution as a native Windows/macOS/Linux app. Unzip and run `npm install && npm start` to launch, or `npm run build` to package.

---

## Running Locally

Double-click `BoomRockChess.html` or open it in any modern browser. No server or dependencies required for single-player and local two-player.

For networked multiplayer, host the file on any static server with WebSocket support.

---

## File Structure (App Package)

```
BoomRockChess-App/
├── BoomRockChess.html      # The complete game (single file)
├── main.js                 # Electron entry point
├── package.json            # Electron dependencies & build config
├── build-local.bat         # Windows build script
├── assets/
│   └── icon.ico            # App icon
└── .github/workflows/
    └── build.yml           # GitHub Actions CI for packaged releases
```

---

## Credits

Created by **Antonio Modest Tambornino**. The Lawrence Square honours Lawrence Erasmus Peregrine in connection with the Linnean Society.

---

*Scan the QR code (BoomRockChess_QR.svg) to play online.*
