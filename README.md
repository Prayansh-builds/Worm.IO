# Glow Worm

A fast, colourful worm-arena game for phones and computers, in the style of Worm.io and Snake. You steer a glowing worm around a round arena, eat light orbs to grow, and try to trap other worms so they crash into your body.

The whole game is one HTML file with no libraries, so it loads quickly and runs in any modern browser.

## How to play

- **Goal:** get as long as possible without popping.
- **Eat orbs** to grow longer.
- **Trap other worms.** If a worm hits your body, it bursts into orbs for you to eat.
- **Don't hit** the arena wall or the body of another worm. You pop and the game ends.
- **Boost** to dash forward. It costs a little length and drops orbs behind you, so use it carefully.

### Controls

| Device | Steer | Boost |
|---|---|---|
| Phone or tablet | Drag your finger | Hold the Boost button |
| Computer | Move the mouse, or use the arrow keys / WASD | Hold Space or click |

## Features

**Power-ups** (they appear as glowing rings on the map):
- **M, Magnet:** pulls orbs toward you for 8 seconds.
- **S, Shield:** absorbs one crash or wall hit.
- **G, Ghost:** pass through other worms for 6 seconds.

**Smarter computer worms:** they eat orbs, run away from bigger worms, chase smaller ones, aim ahead of your head to cut you off, boost to catch you, and steer around bodies and walls.

**Skins:** unlock new worm looks by reaching higher best scores.

| Skin | Unlocks at best score |
|---|---|
| Sky | Start |
| Sunset | 400 |
| Candy | 1200 |
| Rainbow | 2500 |
| Gold | 4500 |

**Themes:** Meadow, Desert, Candy, Ocean and Neon. Pick one on the start screen. Each changes the background, orb colours, enemy colours and the interface.

**Sound:** effects for eating, power-ups and crashes, plus a gentle generated background tune. All sounds are made in the browser, so there are no audio files. A button in the bottom-left corner mutes everything.

**Scores:** your name, your best score, your chosen skin and theme, and a "Best on this device" top 5 are saved in the browser.

## Game modes

- **Play offline:** solo against 9 computer worms. This works anywhere with no account.
- **Multiplayer:** create a lobby to get a 4-character code, or enter a friend's code to join. A lobby holds up to 10 players, and everyone presses Start when ready. Multiplayer and the shared online leaderboard run through claude.ai, so every player needs to be signed in to claude.ai and have the page open. In multiplayer, orbs are not shared between players yet, so you share the arena but not the same orbs.

## Built with

- HTML5 canvas for all the graphics, with glow, particles and a camera that follows your worm
- Plain JavaScript, no frameworks or libraries
- Web Audio API for sound
- `localStorage` for saved settings and scores

## Project files

- `www/index.html` is the entire game: the page, the styles and the code.

## Ideas for later

- Orbs shared between players in multiplayer
- A global leaderboard on a dedicated server
- More skins, power-ups and arena themes
- Music that changes with the action
