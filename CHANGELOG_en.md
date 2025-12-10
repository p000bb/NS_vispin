# 1.0.0
- Initial release

# 1.1.0
Features
- Add automatic update function

# 1.1.1
Features
- Add system tray
- Optimize the length logic of the pin function dropdown to avoid overflow issues
- Optimize the direction of bottom pin text display to match the direction of top pin text display

Fixes
- Fix the issue that the EXTI column is missing when exporting Excel
- Fix the issue that the pin function conflict detection fails due to the presence of spaces in the pin data when parsing the chip data
- Fix the issue that the EXTI function of some combined pins cannot be displayed properly

# 1.1.2
Features
- Optimize the display of pin names, now it will automatically adapt the text size according to the content

Fixes
- Fix the issue that the pin data is not updated when switching the chip data, resulting in incorrect statistics data
- Fix the issue that the pin data is not updated when switching the chip data, resulting in incorrect detection results

# 1.1.3
Features
- Add hover tooltip for pin functions, when hovering over a pin, the pin function will be displayed

Fixes
- Fix the issue that the program path cannot be updated normally under Chinese path

# 1.1.4
Features
- Add support for EXTI secondary menu selection, optimize the display form of EXTI

# 2.0.0
Features
- Add support for BGA format chip

# 2.0.1
Features
- Add support for BGA format pin spacing ratio configuration
- Optimize the alphabetical ascending display form of BGA format, default to skip some letters according to industry standards, and support double letter display
- Optimize the font size of the selected text of BGA format pins, adjust according to the chip size and pin spacing ratio configuration

Fixes
- Fix the issue that the chip is empty when ctrl_z is undone in some cases

# 2.0.2
Features
- Improve the hover tooltip text introduction function

Fixes
- Fix the issue that the pin configuration color switching is stuck
