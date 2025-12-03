

About this fork

This is a custom fork of MAME, modified so that Atari COPS runs properly using real game data.
The original MAME source marks the COPS game as NO_DUMP, which prevents it from loading ROMs.
In this fork, those restrictions were removed and replaced with the necessary lines so the game can load and execute using my own ld and cd chd files.

Only the essential sections of the driver were changed — all unrelated code in MAME was left untouched.
The goal of the fork is to allow Atari COPS to boot and run while keeping the rest of the MAME source exactly as intended.

What is MAME?

MAME is a multi-system emulation framework focused on the preservation of digital history.
It documents vintage hardware behavior, and its software execution validates the accuracy of that documentation.
MAME combines arcade systems, consoles, computers, calculators, and other digital devices into one unified, open-source environment.

Why this fork exists

The official MAME project cannot enable hardware marked as NO_DUMP unless complete public ROMs exist.
This fork simply enables support for COPS by:

Removing the NO_DUMP restrictions

Allowing the game to load externally supplied ROMs

Keeping all other MAME features intact


This fork is not intended to replace MAME — only to enable this specific hardware for personal research and testing.

Building

This fork compiles exactly like upstream MAME.
Standard commands still apply:

make

or

make SUBTARGET=tiny

Windows users may build with the official MinGW-w64 environment or generate Visual Studio 2022 project files:

make vs2022

License

This fork follows the same licensing terms as upstream MAME:

The project as a whole is released under GPL-2.0+

Most files are licensed under the BSD 3-Clause License


All modifications follow the licensing guidelines of the original project.

