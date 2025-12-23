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

# 2.0.3
Features
- Improve the style of the starting position marker point of the pin of the BGA format, add support for the starting position marker point of the BGA format
- Optimize the calculation of the font size ratio and the pin spacing ratio in the chip configuration in the case of high pin count, avoid calculation lag
- Optimize the blur issue of PNG and PDF download in the case of high pin count

Fixes
- Fix the EXTIx interrupt value logic, where x is changed from reading the last group of numbers in the pin name to reading the first group of numbers in the pin name
- Fix the issue that the pin function dropdown list function contains spaces, currently all spaces are removed

# 2.0.4
Fixes
- Fix the issue that the EXTIx interrupt value logic is incorrect, where x is changed from reading the last group of numbers in the pin name to reading the first group of numbers in the pin name
- Fix the issue that the pin function dropdown list function contains spaces, currently all spaces are removed

# 2.0.5
Features
- Add batch delete project function

Fixes
- Fix the issue that the NRST pin function cannot be selected
- Fix the issue that the EXTIx value is incorrect, now it will accurately read the numbers in the pin name

# 2.0.6
Fixes
- Fix the issue that the checkbox in the conflict configuration is not selected
- Fix the issue that the EXTI line conflict detection fails

# 2.0.7
Fixes
- Fix the issue that the secondary EXTI option display is abnormal under different format pin names
- Fix the issue that the button text of the alternative solution under the conflict details is displayed incorrectly

# 2.0.8
Fixes
- Fix the issue that the pin search flashes when switching the chip data

# 2.0.9
Features
- Add desktop update log function, click the version number to view the update log