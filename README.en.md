 [简体中文](./README.md) | English
 
# Chip Pin Visualization Configuration System

## Project Introduction

This web application is a chip pin visualization configuration system based on encrypted chip data provided by Nationz Technology, primarily used for:

- **Online Visual Configuration**: Configure chip pin functions through an intuitive visual interface
- **Project Management**: Support multi-project management for maintaining chip data across different projects
- **Conflict Detection**: Real-time detection of pin function conflicts with intelligent prompts
- **Data Export**: Support exporting in multiple formats including Excel, SVG, PNG, PDF, etc.

## Business Process

1. Access the `html` page using a browser to enter the chip pin visualization configuration page
2. Select the chip to be configured on the page (**chip data is encrypted data provided by Nationz Technology**)
3. Assign pin functions on the page

## 📖 User Guide

### 1. Project Management

#### Create New Project

1. Click the **"New Project"** button on the homepage
2. Enter project name (required) and notes (optional)
3. Click the **"Upload TXT"** button to upload encrypted chip data
4. Click **"Confirm"** to save the project

### Edit Project

1. Click the **edit button** on the project card in the project list
2. Modify project name or notes
3. Click **"Confirm"** to save changes

#### Delete Project

1. Click the **delete button** on the project card in the project list
2. Confirm the delete operation (**this will also delete all chip data under this project**)

---

### 2. Chip Data Management

#### Parse Chip Data

1. Click the **"Upload TXT"** button to upload encrypted chip data
2. The system will automatically parse the data and display it in the chip list

#### Delete Chip Data

1. Click the **delete button** on the right side of the corresponding chip in the chip list
2. Confirm the delete operation
3. After saving the project, the chip data will be automatically deleted

---

### 3. Pin Configuration Preview

#### Search Pins

Enter keywords in the search box on the top left of the preview page. The system will search in the following locations:

- **Pin Names** (e.g., PA0, PB1)
- **Pin Digital Functions** (Digital function list)
- **Pin Analog Functions** (Analog function list)

**Search Features:**
- Search starts after entering at least 2 characters
- Matching pins will highlight and flash for 5 seconds
- Supports real-time search

#### Switch Chip

Select other chips under the project from the dropdown box on the right side of the search box to switch and view pin configurations of different chips.

#### Select Pin Function

1. **Click Pin**: Click any pin in the chip diagram in the center
2. **Select Function**: Select the function to assign from the popup dropdown menu
   - **Common**: Common functions (Reset, Input, Output, EXTI) `Blue border`
   - **Digital**: Digital function list `Green border`
   - **Analog**: Analog function list `Red border`

3. **Confirm Selection**: Click the function option to complete assignment

#### Conflict Detection

The system will detect pin function conflicts in real-time:

- **Conflict Warning**: If the selected pin function conflicts with other pins, the conflict option will be highlighted with a **yellow background** in the dropdown menu
- **Conflict Confirmation**: When clicking a conflict option, the system will pop up a confirmation dialog showing conflicting pin information
- **Conflict Highlighting**: Conflicting pins will flash in **red** on the chip diagram
- **Conflict Details**: View all conflict details in the **"Info"** panel in the bottom right toolbar

#### Clear Pin Function

Select the **"Reset"** option in the pin function dropdown menu to clear the function assignment for that pin.

---

### 4. Toolbar Functions

The preview page provides the following tools in the bottom right corner:

#### 🔄 Undo/Redo

- **Undo**: Undo the last operation (Shortcut: Ctrl+Z)
- **Redo**: Redo the undone operation (Shortcut: Ctrl+Y)
- Supports multi-level undo/redo

#### 🔍 Zoom and Drag

- **Zoom**: Use mouse wheel to zoom the canvas
- **Drag**: Hold Space and left mouse button to drag and move the canvas
- **Reset Layout**: Reset canvas layout to default state (Shortcut: Ctrl+0)

#### ⚙️ Settings

Click the settings button to open the configuration panel:

**Chip Configuration:**
- **Chip Scale**: Adjust chip size (0.5x - 2.0x)
- **Font Size**: Adjust pin name font size
- **Start Position**: Select pin number start position (top-left/top-right/bottom-right/bottom-left)
- **Start Direction**: Select pin number start direction (clockwise/counterclockwise)
- **Chip Sides**: Select number of chip sides (2 sides/4 sides)

**Pin Configuration:**
- **Digital Function Color**: Customize the color of digital function pins
- **Analog Function Color**: Customize the color of analog function pins
- **Common Function Color**: Customize the color of common function pins
- Colors can be customized according to personal preferences

#### 🖥️ Fullscreen/Exit Fullscreen

- **Fullscreen**: Click the fullscreen button to enter fullscreen mode
- **Exit Fullscreen**: Click the exit fullscreen button in fullscreen mode to exit

#### 💾 Download

Click the download button to open the download panel, supporting export in the following formats:

**Excel Export:**
- Export all chip configurations of the current project
- Includes pin information, function selections, etc.
- Supports merging and exporting multi-chip data

**SVG Export:**
- Export in vector graphics format
- Can be scaled without loss, suitable for printing and documentation

**PNG Export:**
- Export in bitmap format
- Suitable for screenshots and quick sharing

**PDF Export:**
- Export PDF documents
- Suitable for formal document archiving

#### 🔄 Restore Default

Click the restore default button to restore all pin configuration values for the current chip

#### 📊 Info Panel

Click the info button to open the info panel, containing two tabs:

**Statistics:**
- Total number of pins
- Number of used pins
- Number of unused pins
- Number of conflicting pins
- Statistics by pin type (Digital/Analog/Common)

**Conflict Details:**
- Display all pin conflict situations
- List conflicting pin pairs
- Provide conflict reason explanations
- Support quick location of conflicting pins

**Conflict Configuration**
- Function conflict detection:
  - The same function cannot be assigned to multiple pins
- EXTI interrupt line conflict detection:
  - The same EXTI line cannot be assigned to multiple pins

#### 🗃️ Renderings
<table>
<tr>
<td>
<img src="https://gcore.jsdelivr.net/gh/p000bb/Image/NTFx/image-1.png">
</td>
<td>
<img src="https://gcore.jsdelivr.net/gh/p000bb/Image/NTFx/image-2.png">
</td>
</tr>
<tr>
<td>
<img src="https://gcore.jsdelivr.net/gh/p000bb/Image/NTFx/image-3.png">
</td>
<td>
<img src="https://gcore.jsdelivr.net/gh/p000bb/Image/NTFx/image-4.png">
</td>
</tr>
</table>