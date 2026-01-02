# GGn Can Make

A Tampermonkey/Greasemonkey userscript for GazelleGames.net (GGn) that shows players what items they can craft based on their current inventory.

## Features

- **READY Tab**: Shows all recipes you can craft right now with current inventory
- **NEED Tab**: Shows recipes you're close to being able to craft (missing 3 or fewer items)
- **REPAIR Tab**: Shows equipment sorted by durability - broken items first, items closest to breaking next
- **FAVS Tab**: Quick access to your favorite recipes
- **PLAN Tab**: Queue up crafts to plan ahead
- **GOALS Tab**: Set goals for items you want to craft
- **BOOKS Tab**: Browse recipes by recipe book
- **INV Tab**: View your current inventory
- **STATS Tab**: Crafting statistics and history

## Installation

1. Install [Tampermonkey](https://www.tampermonkey.net/) (Chrome, Firefox, Edge) or [Greasemonkey](https://www.greasespot.net/) (Firefox)
2. [https://greasyfork.org/en/scripts/560668-ggn-crafter]
3. Navigate to GGn's inventory or crafting pages
4. The panel will appear on the right side of the screen

## Repair Tab

The REPAIR tab shows all your equipment that has repair recipes available, sorted by urgency:

- **BROKEN** (red): Equipment has already expired and needs immediate repair
- **Critical** (yellow): Less than 7 days remaining
- **Warning** (orange): Less than 14 days remaining
- **OK** (green): More than 14 days remaining

When you use any repair recipe (from any tab), the script automatically prioritizes broken equipment first.

## API Key

Some features require a GGn API key:
1. Go to your GGn user settings
2. Generate an API key with "Items" permission
3. Enter it in the OPTIONS tab of the panel

## Development

This is a single-file userscript. To develop:
1. Install in Tampermonkey/Greasemonkey
2. Edit locally and refresh the GGn page to test changes
3. No build step required

See [CLAUDE.md](CLAUDE.md) for technical details about the codebase structure.

## License

MIT
