# Geofence Treasure Hunt Validator

This is a lightweight JavaScript-based geofencing checker for treasure hunts built with Typeform.

## How It Works

- Typeform redirects to this app between questions.
- This app checks if the player is near the specified location.
- If verified, it redirects to the next Typeform question.
- Players can also skip validation.

## URL Format

https://yourusername.github.io/geofence-checker/?game=gameId&question=qX


## Config

Edit `checkpoints.json`:

```json
{
  "gameId": {
    "q1": {
      "lat": 52.xxxx,
      "lng": 13.xxxx,
      "radius": 60,
      "next": "https://typeform-link.com/q2"
    }
  }
}
