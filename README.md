# Polybar bluetooth module
A fully functional bluetooth module for polybar that adds an icon that changes dinamically accordingly to the bluetooth status.

![on](https://github.com/msaitz/polybar-bluetooth/blob/master/screenshots/on.png) When the bluetooth is on

![off](https://github.com/msaitz/polybar-bluetooth/blob/master/screenshots/off.png) When the bluetooth is off

![connected](https://github.com/msaitz/polybar-bluetooth/blob/master/screenshots/connected.png) When the bluetooth is connected to a device

## Dependencies
- Font Awesome 5 Free
- Systemd
- Blueberry

## Installation

Place the shell script files in your preferred sctipt directory.

Add  the module to your polybar config file
```ini
[module/bluetooth]
type = custom/script
exec = path/to/scripts/bluetooth.sh
interval = 2
click-left = exec blueberry
click-right = exec path/to/scripts/config/polybar/toggle_bluetooth.sh
format-padding = 1
format-background = #000000
format-foreground = #ffffff
```
## Usage
Left click on the bluetooth icon launches blueberry or the bluetooth configuration tool of your choice.

Right click on the bluetooth icon toggles the bluetooth power status.
