# PokeBracket
Tool to generate a tournament bracket of Pokemon with various filtering

The goal of this side project was to make a tournament style bracket generator for all Pokemon, with filtering options to allow for smaller more specific pools (Filters outlined below).
I used the PokeAPI to export data and tweaked a custom JSON file, in addition to a JSON containing Pokedex info (used for Region filter and potentially a filter by game later on).  Sprites are also stored locally.

## Overview of Filters:
1. Exclusions - automatically checked and removes things such as Mega evolutions, GMax forms, Costumes (for Pikachu), and other alternative forms (eg. Aegislash has Shield and Blade form).
2. Generation - filters by generation a pokemon was introduced.  Regional forms have been manually changed to show what generation they were introduced in.
3. Region - using the Pokedex JSON, this filters based on which pokemon are obtainable in the selected region
4. Types - filters to pokemon that have the selected type(s).  The "Strict Typing" checkbox makes the filter require a pokemon ONLY have the selected types.
5. Special - filters to Pokemon marked with the specified flags.  Starters will show a dropdown selection for specific starter evolution stages.

## Functionality:
*The "Start Bracket" button will shuffle and generate the bracket based on selected filters.
*The "Auto-shuffle" checkbox will shuffle the pool at the start of each round.
*Undo will undo the last choice, Shuffle Remaining will shuffle the remaining pool.
*Keyboard shortcuts implemented: Left and Right arrow for selecting a winner, U to Undo, and S to Shuffle.
*You can also click on the sprite image to select a winner.
*Below the matchup is a "Match History" that shows prior matchups and winners.
*Once the bracket is over a "Champion" section shows up, showing the winner of the tournament.


Planned future updates:
1. Add types below Pokemon (most likely a checkbox to enable this feature)
2. Add some sort of analytics, at the end of the tournament present information such as: preferred/not preferred types, generation, etc
3. General cleanup of any issues
