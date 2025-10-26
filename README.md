# P7P_charging_unthrottle
Magisk module that raises max temperature for charging - Pixel 7 Pro (Android 16). Obviously your phone needs to be rooted.

I've noticed that my phone would charge very slowly or stop charging altogether if I'm using it at the moment (watching youtube was enough) and it's warm (close to 40C). Turns out there's an overheat protection, which is bit too sensitive.
What I did is I modified system file `/system/vendor/etc/thermal_info_config_charge.json` to add a few degrees to the protection threshold and this is all that was needed.
Feel free to unzip the module and modify the temperatures as you wish.

Here's an example of before and after:

![img1](/screenshot_before.png) ![img2](/screenshot_after.png)

I've used CPU throttling test and covered the phone with a blanket to heat it up for this test. Charging power tapers off above 45C.

Disclaimer: this modifies manufacturer's safety settings and, in theory, can be unsafe. Do this at your own risk. No guarantees or liability.
