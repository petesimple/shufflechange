# Shuffle Change

Shuffle Change is a digital tabletop prototype based on the original Shuffle Change coin flicking game.

Live game:
https://www.shufflechange.com

## What Is Shuffle Change?

Shuffle Change is a two player coin flicking game where players shoot coins across a scoring board, trying to land in the highest value zones while avoiding the gutter.

One player plays Heads.  
One player plays Tails.  

Players take turns flicking coins from the bottom shooting area, known as the kitchen.

First player to 21 points wins, but you must win by 2.

## Current Digital Prototype

This version is built as a single page HTML, CSS, and JavaScript app.

It runs in the browser and is designed for GitHub Pages hosting.

No backend.  
No login.  
No install.  
Just coins, chaos, and questionable physics.

## Features

### Game Board

The board includes:

* Wood style frame
* Green felt gutter
* Scoring lane
* Kitchen shooting area
* Scoring zones of 1, 2, 3, 0, 3, 2, 1
* Midline replay rule
* Gutter scoring rule

### Coin Flicking

Coins are flicked using pointer based controls.

Supported input:

* Mouse
* Trackpad
* Touch screens
* Mobile Safari
* Desktop Safari
* Chrome based browsers

The current flick rule:

1. Touch or click inside the kitchen
2. Flick forward toward the board
3. Release before leaving the kitchen
4. If the coin does not cross the midline, replay the shot
5. If the release is illegal, replay the shot

### Coin Sprites

The prototype uses procedural canvas coin sprites.

This means the coins are drawn in code instead of relying on image files.

Current sprites include:

* Heads coin style for Player A
* Tails coin style for Player B
* Metallic coin shading
* Ridged coin edges
* Ownership color rings
* Visual coin squish during motion

### Physics

Current physics include:

* Flick velocity based on pointer movement
* Friction based sliding
* Coin to coin collision
* Wall bounce
* Gutter drag
* Gutter trapping
* Random coin flipping on hard impacts
* Replays for coins that do not cross the midline

## Rules Implemented

Current prototype assumptions:

* Two players
* Player A is Heads
* Player B is Tails
* Players alternate shots
* Six total coins per round
* Coins must be shot from the kitchen
* Release must happen before leaving the kitchen
* Coins must cross the midline or the shot is replayed
* Coins in the gutter score 0
* Coins touching a gutter coin score 0
* Center zone scores 0
* Line touch scores the lower value
* Flipped coins change owner for the current round
* First to 21 wins
* Must win by 2

## Project Structure

This prototype can be run from a single `index.html` file.

Suggested structure:

```text
shufflechange/
  index.html
  README.md
