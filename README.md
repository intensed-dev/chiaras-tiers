# Points Leaderboard

A simple static leaderboard website using a JSON data file.

## Data structure

Each user has points separated by category:

```json
{
  "username": "User1",
  "categories": {
    "categoryA": 500,
    "categoryB": 100
  }
}
```

The **Overall** leaderboard automatically adds every category:

`500 + 100 = 600 points`

You do not need to store overall points separately.

## Adding a category

Add the category to each user's `categories` object:

```json
"categoryC": 250
```

Then add a leaderboard entry:

```json
{
  "id": "categoryC",
  "name": "Category C",
  "icon": "star",
  "description": "Points earned in Category C."
}
```

The tab and its ranking will be generated automatically.

## Profile images

Minecraft profile heads are loaded from:

`https://render.crafty.gg/2d/head/USERNAME?size=256`

## Running locally

Because the website loads `data.json` with `fetch()`, serve the folder through a local web server instead of opening `index.html` directly.

For GitHub Pages, no build step is required.
