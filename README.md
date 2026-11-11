# Squeek Snack Dash

A game website for Squeekchain: catch game, inventory, and shop — all in one place.

Squeek Snack Dash is a community project for the Squeekchain Buildooooor badge.

## The website

`index.html` is the home of the game — no coding vibe, just a game site:

- **Home**: what Squeekchain is (a real hamster runs the chain), live wheel stats, and the game picker (Snack Dash here, Squeek Fly on its own site).
- **Inventory**: everything you caught, earned and unlocked — snack coins, games played, best score, best combo, badges — saved on your device.
- **Shop**: spend snack coins on hamster looks (Golden, Berry, Mint, Shadow) and one-run boosts (Extra Life, Slow Snacks, Double Points).

Play money only: snack coins are earned by playing, worth nothing, no wallet, no payment.

## The game

`play.html` is the catch game: move the hamster left/right, catch SQK coins (+10), seeds (+5), berries (+15), dodge the cage bars (-1 life). Combo multiplier up to x5, 3 lives, 60 seconds. Your score is banked as snack coins; the skin you wear and the boosts you bought in the shop apply to your next run.

## Live data

The site reads the official public API for the live wheel status:

```
GET https://api.squeekchain.com/v1/status
```

It shows the current block, settled round, wheel distance, and whether Squeektoshi is RUNNING or IDLE. While the real wheel is running, snacks fall 25% faster. If the API is unreachable the game plays at normal speed and says so.

## Run

Static site — no build step, no backend, no wallet, no keys.

```
open index.html
```

## Credits

Squeekchain: https://squeekchain.com (Sepolia testnet).

squeekchain-project: 20ef9490-e374-4f3d-bc98-a077792763f6
