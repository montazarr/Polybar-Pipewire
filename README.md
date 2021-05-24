# Polybar Pipewire

A shell script for switching sink, changing volume, and toggling mute.

> This script is based upon the Polybar shell script by Victortrac on Github.

## Dependencies

- pipewire
- pipewire-pulse

## Module

```ini
[module/pipewire]
type = custom/script
exec = ~/.config/polybar/pipewire.sh
tail = true

label= %output%

click-right = ~/.config/polybar/pipewire.sh previous-sink
click-left = ~/.config/polybar/pipewire.sh next-sink
click-middle = ~/.config/polybar/pipewire.sh toggle-mute
scroll-up = ~/.config/polybar/pipewire.sh volume-up
scroll-down = ~/.config/polybar/pipewire.sh volume-down
```
