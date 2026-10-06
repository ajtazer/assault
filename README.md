# Commando Assault

The old Flash game **Commando Assault**, playable in the browser again.

**Play:** http://play.bihari.xyz · backup: https://ajtazer.github.io/assault

## Where the game is from

Commando Assault is a Miniclip game from around 2010. The game code credits the developer as Macrojoy. I downloaded the original `.swf` file from the web. All rights to the game belong to its creators. This is only a fan-made way to keep playing it.

## How it runs

Browsers dropped Flash years ago. This page uses [Ruffle](https://ruffle.rs), a free Flash emulator that runs inside your browser, so there's nothing to install.

## What I changed

- **Removed the "localhost only" check.** The game has Miniclip's site code built in. On any real website it tried to connect to Miniclip's servers, which are gone, so it got stuck on a black screen. It only skipped that step when opened on `localhost`. I edited one function (`isLocal()`) so the game always thinks it's local, and now it runs anywhere. The edit was made with the [JPEXS Flash decompiler](https://github.com/jindrapetrik/jpexs-decompiler).
- **Made it fill the screen.** The game is set to draw at a fixed small size in the corner. The page tells Ruffle to scale it up to fit the window and center it.

Nothing else in the game was changed.
