# duck-runner
A 3D tower-climbing obstacle game built with Three.js, inspired by the *Twisted System* mini-game from Fusion Frenzy.

You walk up a spiral ramp wrapped around a spinning tower. Obstacles sweep around the tower toward you: jump the low blue bars and duck under the red arms with duck signs. Every hit knocks you back down the ramp, and the eighth hit throws you off into the abyss. The tower keeps speeding up for as long as you survive.

## How to Play

- **SPACE / UP ARROW / W**: Jump over low bars
- **DOWN ARROW / S (hold)**: Duck under duck-sign arms; ducking in mid-air drops you fast
- **P / ESC**: Pause
- **Touch screens**: hold the DUCK button (bottom left), tap JUMP (bottom right)

## Features

- Spiral ramp that turns around the tower, with obstacles coming into view as they round the curve
- 8-hit footing meter; each hit costs you ground on the ramp
- Endless speed-up every 10 obstacles cleared
- Best score saved in your browser
- Mobile-friendly with on-screen buttons

## Play the Game

[Play Duck Runner Now](https://evanmydude.github.io/duck-runner/)

## Development

This game is built using vanilla JavaScript and Three.js without additional frameworks or dependencies. Open the page with `?debug` to expose a `window.__game` hook used for automated testing.
