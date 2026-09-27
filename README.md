# NightRest

A lightweight and configurable Minecraft server plugin that gives server owners control over how sleeping works.

Instead of requiring every eligible player to sleep before the night can be skipped, NightRest lets you define a custom sleep requirement based on a specific number of players or a percentage of eligible players online.

NightRest is designed to keep the player experience simple while providing useful control over sleep requirements, notifications, worlds, localization, permissions, and weather behavior.

## Features

* Configure sleep requirements by player count or percentage.
* Support for single-player sleep.
* Count eligible sleeping players per world or across the entire server.
* Dynamically calculate requirements from players currently online.
* Configure which worlds NightRest operates in.
* Exclude spectators from the sleep count.
* Optionally exclude players with a configurable permission.
* Prevent vanilla night skipping before the configured NightRest requirement is reached.
* Fully customizable sleep and night-skip messages.
* Enable or disable chat notifications.
* Optional silent mode.
* Support for multi-line messages, colors, prefixes, separators, sounds, and placeholders.
* Built-in localization system.
* 9 included languages.
* Use a custom language as the default for the server.
* Configurable rain and thunderstorm behavior.
* Reload the configuration without restarting the server.
* Built-in status, version, and chat testing commands.
* Optional debug mode for troubleshooting.
* No client-side mod required.
* No required third-party plugins.

## How It Works

NightRest replaces the normal requirement for every eligible player to sleep with a configurable requirement.

For example, with two eligible players online and a requirement of `2` sleepers:

```text
Player 1 sleeps
→ 1 player is still needed.

Player 2 sleeps
→ 0 players are still needed.
→ NightRest skips the night.
```

With a requirement of `1` sleeper:

```text
Player 1 sleeps
→ 0 players are still needed.
→ NightRest skips the night.
```

Requirements can be configured using either a fixed player count or a percentage of eligible players.

## Configuration

NightRest is designed to be beginner-friendly. Most settings can be changed directly through `config.yml`, and the included comments explain what each option does.

The default language is `en_US`, and additional language files are included with the plugin.

Configuration can be reloaded without restarting the server.

## Notifications

NightRest can send customizable messages when players start sleeping and when the night is skipped.

Chat notifications can be enabled, disabled, or configured to use different delivery methods depending on the server's needs.

Servers that prefer no sleep-related messages can disable chat notifications or use silent mode.

## Languages

NightRest includes 9 language files by default:

* English (US)
* English (UK)
* Spanish (Argentina)
* Spanish (Spain)
* Portuguese (Brazil)
* French
* German
* Italian
* Russian

Language files can be edited to customize the plugin's messages.

## Commands

The plugin provides simple commands for administration and testing, including:

```text
/nr reload
/nr status
/nr version
/nr testchat
```

Additional administrative commands and options can be configured through the plugin settings and permissions.

## Permissions

NightRest includes permission support for controlling which players are affected by the sleep system.

Permissions can be configured according to the needs of your server.

## Compatibility

NightRest is designed for server-side Minecraft environments that support the plugin's Bukkit/Paper API.

* No client-side installation required.
* No required third-party plugins.
* Java 17+.

## License

NightRest is released under the MIT License.

See the [LICENSE](LICENSE) file for the full license text.
