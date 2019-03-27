# bin-utils
A collection of shell scripts as utilities

Move/Copy the .rules files into your udev rules directory
`sudo cp udev_rules/*.rules /etc/udev/rules.d/`

Use `sudo mv` or `sudo ln -s` to move utility files to a place on the path 
- I use /usr/local/bin
`sudo ln -srfv backlight /usr/local/bin/backlight`
`sudo ln -srfv trackpoint /usr/local/bin/trackpoint`

## Usage
### General Notes
- n is any integer
- Value is capped at the reported maximum brightness for the device
 and floored at 1 (0 turns off the display)

### Backlight
backlight
- Passed without any arguments, gets the raw value of the current backlight

backlight %
- Gets the percentage of the current backlight

backlight n
- Sets the backlight to this raw value

backlight +n
- Increments the backlight raw value by this amount

backlight -n
- Decrements the backlight raw value by this amount

backlight n%
- Sets the backlight to this percentage of the total brightness

backlight +n%
- Increments the backlight percentage by this percentage amount

backlight -n%
- Decrements the backlight percentage by this percentage amount

### Trackpoint
trackpoint
- Passed without any arguments, reports the settings for trackpoint sensitivity and speed

trackpoint s
- Gets the sensitivity of the trackpoint

trackpoint p
- Gets the speed of the trackpoint

trackpoint s n
- Sets the trackpoint sensitivity to n

trackpoint p n
- Sets the trackpoint speed to n

