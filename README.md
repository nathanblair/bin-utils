# bin-utils
A collection of shell scripts as utilities

Use `sudo mv` or `sudo ln -s` to move these files to a place on the path - I use /usr/local/bin

## Usage

### General Notes
- n is any integer
- Value is capped at the reported maximum brightness for the device
 and floored at 1 (0 turns off the display)


backlight
- Passed without any arguments, gets the percentage of the current backlight

backlight n
- Sets the backlight to this raw value

backlight +n
- Increments the backlight raw value by this amount
 
backlight -n
- Decrements the backlight raw value by this amount
 
backlight n%
- Sets the backlight to this percentage of the total brightness

backlight +n%
- Increments the backlight percentage by this amount

backlight -n%
- Decrements the backlight percentage by this amount
 
