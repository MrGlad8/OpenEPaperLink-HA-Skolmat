# OpenEPaperLink-HA-Skolmat
<img src="https://github.com/MrGlad8/OpenEPaperLink-HA-Skolmat/blob/main/Skolmat%20Display%20Example.jpg" width="400">

This automation will keep one of your 2.9'' OpenEPaperLink-displays updated with the food-menu of your selected school with help from the sensor from the skolmat-integration.

This automation will send the todays and tomorrows food-menu of your selected school to the display, updating 03:00 each day monday to thursday.
At friday it will show todays menu and the menu of monday next week. And on saturday/sunday it will change to only show mondays food-menu.

You first need Home Assistant and a working [OpenEpaper](https://openepaperlink.de/) setup. 
And this code is designed for a 2.9'' size display.

# Integrations needed:
* https://github.com/jonasniesner/open_epaper_link_homeassistant (Install via HACS)
* https://github.com/Kaptensanders/skolmat - The skolmat-integration (Install via HACS)

# Installation:
1. Download the font `GothamRnd-Bold.ttf` and place it in your HA-folder: `/media/fonts/`
* (If you want the font elsewhere, be sure to point it to the correct place in the automation-code or you will get an error when the automation is triggered.)  
2. Create a new automation from the `2.9_skolmat_automation.yaml`   
3. Update the automation with the name of your sensors:
* `skolmat.YOUR_SCHOOL`
* `open_epaper_link.YOUR_DISPLAY_NAME`

# For more OpenEPaperLink-projects visit:
* https://github.com/jonasniesner/open_epaper_link_homeassistant/wiki
