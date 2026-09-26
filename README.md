# NightRest

A lightweight and customizable Minecraft server plugin that gives you control over how sleeping works.

Instead of requiring every online player to sleep, NightRest lets you decide how many players—or what percentage of eligible players—must be sleeping before the night is skipped.

NightRest is designed to keep the player experience simple while giving server owners full control over sleep requirements, broadcasts, worlds, localization, and permissions.

---

## Features

- Configure sleep requirements by player count or percentage.
- Count sleeping players per world or across the entire server.
- Configure which worlds NightRest can operate in.
- Exclude spectators from the sleep count.
- Optionally exclude players using a permission.
- Prevent vanilla sleeping from skipping the night before NightRest processes the configured requirement.
- Fully customizable sleep and night-skip broadcasts.
- Multi-line broadcasts with colors, prefixes, separators, sounds, and placeholders.
- Built-in localization system.
- 9 included languages.
- Reload configuration without restarting the server.
- Built-in status, version, test, and debugging commands.
- No client-side mod required.
- No required third-party plugins.

---

## How It Works

NightRest replaces the usual "everyone must sleep" behavior with a configurable requirement.

For example, with two eligible players online and a requirement of `2` sleepers:

```text
1/2 players sleeping
→ The night continues.

2/2 players sleeping
→ NightRest skips the night.
