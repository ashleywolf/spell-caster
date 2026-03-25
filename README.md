# :crystal_ball: Spell Caster

Defend your tower by yelling spell names at your screen. Speech recognition mishears are half the fun.

## [Play Now](https://ashleywolf.github.io/spell-caster/) (Chrome/Edge)

## What Is This

Voice-controlled tower defense. Enemies march toward your tower and you fight them off by shouting spell names into your microphone. Say "FIREBALL" and fire flies. Say "FREEZE" and they slow down. Say something the game doesn't recognize and you get a chaos spell, which could save you or end you.

## Features

- 5 known spells: FIREBALL, SHIELD, LIGHTNING, FREEZE, HEAL
- Chaos spells for any unrecognized word (the speech API's mistakes become a game mechanic)
- Spell combos: SHATTER (freeze + fireball, 3x damage), SURGE (lightning + shield, chain), PHOENIX (heal + fireball, homing)
- Wave countdown with enemy preview so you can plan your yelling strategy
- Live transcript showing what the speech API thinks you said (often hilarious)
- Post-game stats breakdown of spells cast, accuracy, and combo count
- Ambient drone that builds tension between waves
- Screen flash on tower damage
- localStorage high scores

## How to Play

- Enemies approach your tower in waves. Shout a spell name to cast it.
- Combine spells for combos: freeze an enemy, then fireball it for SHATTER (3x damage).
- Say anything weird for a random chaos spell. Sometimes it works. Sometimes it really doesn't.
- Survive 5 waves and the boss fight. Your voice is your only weapon.

## Tech

- Web Speech API with continuous recognition and interim results
- Real-time speech-to-text matching against spell dictionary
- Combo detection tracking last 2 spells within a time window
- HTML5 Canvas for tower defense rendering

## Browser Support

Chrome or Edge required (Web Speech API). Microphone access needed. Works best when you commit to actually yelling.

## Part of Browser Party Games

8 single-file browser games built with MediaPipe, Transformers.js, Web Audio, and Web Speech. No servers, no build steps, no installs.

| Game | Input | Tech |
|------|-------|------|
| [Type or Die](https://ashleywolf.github.io/type-or-die/) | Keyboard | Vanilla JS |
| [Grin Sweeper](https://ashleywolf.github.io/grin-sweeper/) | Smile (webcam) | MediaPipe Face |
| [Show & Tell](https://ashleywolf.github.io/show-and-tell/) | Real objects (webcam) | Transformers.js DETR |
| [Pitch Climber](https://ashleywolf.github.io/pitch-climber/) | Voice pitch (mic) | Web Audio API |
| [Spell Caster](https://ashleywolf.github.io/spell-caster/) | Shout spells (mic) | Web Speech API |
| [Stone Face](https://ashleywolf.github.io/stone-face/) | Don't react (webcam) | MediaPipe Face |
| [Ninja Hands](https://ashleywolf.github.io/ninja-hands/) | Hand tracking (webcam) | MediaPipe Hands |
| [Duck & Cover](https://ashleywolf.github.io/duck-and-cover/) | Duck + yell (webcam+mic) | MediaPipe Pose + Web Audio |

---
Built with vanilla JS + browser ML. Each game is one HTML file. Fork it, break it, make it yours.
