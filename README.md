# duck-runner
A 3D tower-climbing obstacle game built with Three.js, inspired by the *Twisted System* mini-game from Fusion Frenzy.

You walk up a spiral ramp wrapped around a spinning tower. Obstacles sweep around the tower toward you: jump the low blue bars and duck under the red arms with duck signs. Every hit knocks you back down the ramp, and the eighth hit throws you off into the abyss. The tower keeps speeding up for as long as you survive.

## How to Play

- **SPACE / UP ARROW / W**: Jump over low bars
- **DOWN ARROW / S**: Duck under duck-sign arms. You stay down while the key is held, for at most about half a second, so press once per arm; a press held through a landing ducks as soon as you land
- **P / ESC**: Pause
- **Touch screens**: tap DUCK (bottom left) and JUMP (bottom right)

## Features

- Spiral ramp that turns around the tower, with obstacles coming into view as they round the curve
- Voiced "Get ready... 3, 2, 1, GO!" intro with synced countdown text; the tower starts turning and controls go live on GO, then the cue crossfades into the music
- 7-hit footing meter; each hit costs you ground on the ramp
- Jumps are committed: once you leave the ground you ride the arc until you land
- Continuous speed-up: the tower turns faster and obstacles come closer together with every obstacle you reach. 100 is a good score; 200 is close to the human limit
- Never impossible: obstacle spacing has a hard floor derived from the jump physics, and on which obstacle types come in a row, so every sequence stays clearable with perfect inputs, even at top speed
- Best score saved in your browser
- Mobile-friendly with on-screen buttons

## Play the Game

[Play Duck Runner Now](https://evanmydude.github.io/duck-runner/)

## Development

This game is built using vanilla JavaScript and Three.js without additional frameworks or dependencies. Open the page with `?debug` to expose a `window.__game` hook used for automated testing. To practice the late game, run `__game.startAt(150)` in the console, then press Start.
