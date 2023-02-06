# Automatically disable the Xbox One/Series S/X Controller LED

This is a udev rule that turns off the Xbox One/Series S/X Controller LED upon connecting it to the system using the xone driver by medusalix. 

Put this rule in /etc/udev/rules.d and remember to run udevadm control --reload as the root user to enable it.

There is no other way to easily turn off this LED without opening the controller and desoldering it.

This method is pretty much the best since it doesn't tamper with the hardware and it also allows the LED to blink when it is searching for a host to conenct to, so you only see the LED when you need to see it.

I haven't seen this udev rule thing documented anywhere, not even in the xone driver page (it only mentions how to disable the LED manually using a command that does this exact thing, but no automatic method is provided) so for the sake of keeping it around (since I REALLY HATE BLIND LEDS ON MY FACE!) I'm uploading it here.
