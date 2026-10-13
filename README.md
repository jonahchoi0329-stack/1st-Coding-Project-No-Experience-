# Wildlight — your first coding project

An original, small 2D adventure inspired by the exploration and discovery of open-world adventure games. Explore a green valley, find three crystals, fight guardians, and awaken an ancient beacon. This is a beginner-friendly prototype, not a full 3D Breath of the Wild replica.

## Play

Open `index.html` in Chrome, Firefox, Edge, or Safari. There is nothing to install.

Alternatively, from this project folder run:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser. Stop the server with Ctrl+C.

## Controls

| Action | Control |
| --- | --- |
| Move | WASD or arrow keys |
| Sprint | Hold Shift (uses stamina) |
| Swing sword | Space (uses stamina; face your enemy) |
| Collect, heal at campfire, or activate beacon | E |
| Pause | Escape or Pause button |

On small screens, use the on-screen movement, sword, and E buttons. Golden dots on the map are crystals; the orange dot is your campfire. Find all three crystals, then interact with the beacon in the north. If you lose all hearts, you return to camp and keep your crystals.

Your progress saves in this browser automatically when storage is available. Use **New adventure** to start over. Browser storage can be cleared, so this is not a cloud save.

## Learn by changing one thing

- `index.html`: the page's structure, title, and buttons.
- `style.css`: the interface's colors, fonts, and layout.
- `game.js`: movement, combat, world drawing, and saving. No game engine or packages required.

Try changing `145` in `const speed=sprint?250:145` to `180` in `game.js`. Save and refresh: your walking speed increases. Next, try moving a crystal by changing its `x` and `y` at the top of that file. The world is 2400 pixels wide and 1800 pixels tall.

All graphics are drawn with code, and the world and characters are original. Future projects could add sound, new quests, gamepad controls, or a 3D world.
