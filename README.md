[README (4).md](https://github.com/user-attachments/files/26170830/README.4.md)
# Poetry Dash 🎮

A Geometry Dash-inspired poetry runner. Dodge words of silence, collect words of light.

## Play

Open `poetry-dash.html` in any browser. No install, no build step, no dependencies.

## Controls

| Input | Action |
|-------|--------|
| `Space` | Jump |
| Click / Tap | Jump |
| Double press | Double jump (mid-air) |

## How it works

- Your cube auto-scrolls through three **Cantos**, each faster than the last
- **Red blocks** = bad words (`silence`, `void`, `doubt`) — touch one and you die
- **Gold orbs** = collectible words (`light`, `dawn`, `fire`) — grab as many as you can
- Complete all 8,000 units to win

## Cantos

| # | Speed | Theme |
|---|-------|-------|
| Canto I | 5.5× | Purple — hope and breath |
| Canto II | 7× | Cyan — tide and dream |
| Canto III | 9× | Amber — fire and ash |

## Customisation

All game data lives in the `LEVELS` array near the top of the script:

```js
const LEVELS = [
  {
    name: "CANTO I",
    speed: 5.5,
    bg: ['#0d001f', '#1a0035'],
    accent: '#b47aff',
    obstacles: ['silence', 'void', 'prose'],
    collectables: ['light', 'dawn', 'breath', ...],
    poem: ["line one", "line two", "line three"]
  },
  // ...
];
```

Add a new object to the array to add a new Canto.

## Files

```
poetry-dash.html   ← the entire game
README.md          ← you are here
```
