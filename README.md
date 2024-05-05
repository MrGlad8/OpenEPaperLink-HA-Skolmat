# OpenEPaperLink-HA-Skolmat
This automation will keep one of your 2.9'' displays updated with the food-menu of your selected school.

This automation will send the todays and tomorrows food-meny to the display updating 03:00 each day monday to thursday.
At friday it will show todays meny and the menu of monday next week. And on saturday it will change to only show mondays menu.

# Integrations needed
* The OpenEPaperLink-integration: https://github.com/jonasniesner/open_epaper_link_homeassistant (Install via HACS)
* The skolmat-integration: https://github.com/Kaptensanders/skolmat (Install via HACS)

# Initial setup
1. Download the font "GothamRnd-Bold.ttf" and place it in your: /media/fonts/
* (If you want the font elsewhere, be sure to point it to the correct place in the automation-code or you will get an error when the automation is triggered.)  
2. Create a new automation from the 2.9_skolmat_automation.yaml   
3. Update the automation with the name of your sensors:
* skolmat.YOUR_SCHOOL
* open_epaper_link.YOUR_DISPLAY_NAME
