# Hi, I'm Andre Mendoza! 👋

## About Me
Currently taking CSC-113 AI Fundamentals and learning to collaborate with AI tools!

## My Foo 🎯
My passion is for video games and video game art, and I am already practicing how to draw landscapes and abstract art before learning how to draw realisitc bodies.

## Currently Learning
- 🤖 AI collaboration and prompt engineering
- 🐙 GitHub workflows and version control
- 💡 Building my first AI assistants

## Fun Fact
I've managed to 100% Every 3D Zelda game from Ocarina of time all the way to Skyward Sword, BOTW is too big to finish as a full time student. So is TOTK!

## Find Me
- 📫 Right here on GitHub!

# Pokemon Team Generator MVP

## What It Does
The Pokémon Team Generator is a web application designed to help competitive Pokémon players quickly build balanced 6-Pokémon teams based on common formats (like OU or VGC) and strategic styles (like Balanced or Offensive). It automatically suggests optimized EV spreads (Effort Values) and Natures for each Pokémon based on their role (Tank, Special Attacker, Physical Attacker) and category.

## How to Use
1. Select Format: Choose a competitive tier, like "OU" (OverUsed) or "VGC" (Video Game Championship), from the first dropdown.
2. Select Style: Choose a strategy, such as "Balanced" for a mix of defensive/offensive roles, or "Offensive" for hyper offense.
3. Generate Team: Click the "Generate Team" button. The app selects six Pokémon from the available pool, checking to avoid major, overlapping type weaknesses (e.g., preventing a team from having four Pokémon weak to Ground).
4. Review Output: The generated Pokémon are displayed. Below the list, the full Showdown/Smogon export text appears, ready to be copied.
Copy & Export: Click "Copy Team" to instantly paste the text into a simulator like Pokémon Showdown.

## Features Implemented
Dynamic Role-Based EV/Nature Assignment: Assigns specific EV spreads and Natures based on the Pokémon's role and category:

Tanks/Support: 252 HP / 252 SpD / 4 Def with Calm Nature (+SpD, -Atk).

Special Attackers: 252 SpA / 4 Def / 252 Spe with Modest Nature (+SpA, -Atk).

Physical Attackers: 252 Atk / 4 Def / 252 Spe with Adamant Nature (+Atk, -SpA).

Weakness Balancing: A core constraint check prevents the generation of teams with egregious, shared four-way type weaknesses (e.g., too many Pokémon weak to Water or Ground).

Dark Mode Toggle: A user-friendly toggle that saves the user's theme preference to localStorage and respects system preference on initial load.

## Try It Yourself
[Link to GitHub Pages deployment]

## What I Learned
I gained a deeper understanding of algorithm complexity in constrained data selection. Implementing the type weakness constraint and the role-filling logic required careful iteration and filtering to ensure the pool wasn't prematurely exhausted, especially when dealing with smaller pools like VGC.

## Future Improvements
Move/Ability Suggestion: Populate the [Move 1], [Item Placeholder], and [Ability Placeholder] fields with the Pokémon's most common competitive choices, adding significant utility.
Team Analysis Display: Show a visual type-weakness chart for the generated team to provide immediate feedback on defensive coverage.
Filtering by Type: Add a filter that allows the user to ensure a specific type (e.g., Steel) or hazard remover is included in the final team.
Database Scaling: Transition the current static POKEDEX array to a simple, external JSON file or a lightweight database to facilitate easier expansion of the Pokémon roster.
