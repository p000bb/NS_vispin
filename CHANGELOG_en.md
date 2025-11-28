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