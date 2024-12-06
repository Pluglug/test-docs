Original:
https://archive.blender.org/wiki/2015/index.php/User:Raa/Addons/Pie_Menu_Editor/


Document Design Proposal

Pending due to need to consider compatibility with `PME_OT_docs`

# Getting Started
## About Pie Menu Editor
## Installation
## Version Compatibility
  - Support for Blender 4.0+
    Related: FAQ: How to Apply Patches
## Current State & Contribution

---

# Basic Usage Guide
  - Quick Tutorial
  - Create Your First Menu
  - Common Use Cases

---

# Customization & Editors
## Editors
### Pie Menu Editor
Allows to create nested pie menus with 8+ buttons.
### Regular Menu Editor
Allows to create multi-column menus which can be called by using the assigned hotkey or used as a sub-menu. (BPY.TYPES.MENU)
### Pop-up Dialog Editor
Allows to create a layout of widgets that can be displayed in pie menus, dialogs, panels or toolbars. (BPY.TYPES.PANEL)
### Sticky Key Editor
Hotkeys can be set to have different actions when pressed or released, which is useful for temporarily activating a tool or mode.
### Stack Key Editor
Allows to stack commands and cycle between them using the assigned hotkey.
### Macro Operator Editor
Allows to create new tools using existing Blender tools without coding.
### Modal Operator Editor
Allows to create interactive tools.
### Property Editor
Allows to create custom properties (widgets).

### Editor Common Elements
#### Hotkeys
  - Hotkey Mode
      - Press: Press the key
      - Hold: Hold down the key
      - Tweak: Hold down the key and move the mouse
      - Double Click: Double click the key
#### Slot Editor
  - Command Tab
      Python code that will be executed when the user clicks the button.
      `print("Hello World!")`
  - Property Tab
      Path to the object's property which will be displayed as a widget.
      `bpy.context.object.name`
  - Menu Tab
      Open/execute the menu, popup or operator when the user clicks the button. Or draw a popup dialog inside the current popup dialog or pie menu.
  - Hotkey Tab
      ender's hotkey that will be used to find and execute an operator assigned to it when the user clicks the button.
  - Custom Tab
      Python code that will be used to draw custom layout of widgets.
      `L.box().label(text, icon=icon, icon_value=icon_value)`
#### Poll Method (Advanced Settings)
(Advanced Settings exist for each editor, but Poll is a common and important element.)

## UI Customization
### Panel Group (Side Panel Editor)
Allows to create a group of panels and add it to the new or existing category (tab).
### Hiding Unused Panels
The editor allows to hide a group of panels.
### PME Toolbars (Pop-up Dialog Editor)
This appears when you narrow the area of ​​Blender's Preference Editor to a certain extent, and you can place custom buttons. It can be identified when the menu name of the Popup Dialog is "Toolbar Layout Left" or similar.
### Menu/Panel Extension (Pop-up Dialog Editor/Regular Menu Editor)
Appends or prepends a PME item to any panel/menu in Blender. It is identified when the menu name of the PME item is an ID such as "USERPREF_HT_header".
Related: Interactive Panels Mode


## Adding Widgets
### RMB Context Menu
  1. RMB Template-RMB.png on some widget
  2. Pie Menu Editor » Add as Button
  3. Select the slot for the widget
  Some widgets don't support this method.
### Last Action
  1. Do some action in Blender
  2. Ctrl+Shift+Accent grave (PME Hotkey 関連: Settings)
  3. Select the slot for the last action.
  Some actions don't support this method.
### Info Area
  1. Select some actions in Info area
  2. Ctrl+Shift+Accent grave
  3. Select the slot for the selected actions.
### Editor
  Using Slot Editor you can add almost any widget to the menu.

## Settings
 - General
 - PME Hotkeys
 ...
 - Debug Mode
    Actively log in the info area or console
 - Interactive Panels Mode
    A PME Tools button has been added to all UI elements in Blender, making it easy to get menu IDs, set up Extending Panels, etc.
## Custom icon
If you store an icon image in pie_menu_editor/icon, you can use it as a custom icon in PME.

---

# Reference
## Terminology
## PME Scripting Reference
### Global Variables
### Global Functions
#### Common Functions
#### Command Tab Functions
#### Custom Tab Functions
### Auto-run Scripts
### Creating Custom Globals

---

# Scripting Guide
<!-- ## Blender Basics -->
  <!-- - Understanding Blender's UI -->
  <!-- - Data Structure -->
  <!-- - Operator System -->
  <!-- - Keymap System -->
  <!-- - Poll System -->
## Python Essentials
  - Core Concepts
  - List Comprehensions
  - Ternary Operators
  - Best Practices
## BPY Guide
  - Context & Data Access
  - Operator Usage
  - UI Layout System
  - Area Management

---

# Examples & Community Resources
## Basic
  - Menu Creation
  - Panel Extensions
  - Custom Operations
## Practical
  - Animation Tools
  - Modeling Workflows
  - Scene Management
  - Property Management
  - Event Handling
  - Leverage generative AI

## Script Collection
  - Installation Guide
  - Available Scripts
  - Usage Instructions
  - Contributing Guidelines
## Knowledge Base
  - Tips & Tricks
  - Problem Solving
  - Performance Tips
  - Known Limitations

---

# Support & Community
- Get Support
- Frequently Asked Questions
    How to Apply Patches
- Known Issues
- Contribute to PME
    Bug Reporting
    Script Sharing
    Contribute to the documentation
        Translation Help
- Changelog


pme_docs/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   └── workflows/
│       └── deploy.yml
├── docs/
│   ├── source/
│   │   ├── _static/
│   │   ├── _templates/
│   │   ├── images/
│   │   ├── examples/
│   │   ├── references/
│   │   ├── examples/
│   │   ├── community/
│   │   └── conf.py
│   ├── build/
│   └── Makefile
├── images/
│   ├── banners/
│   └── icons/
├── patches/
│   └── pme_fixes.patch
├── scripts/
│   ├── examples/
│   └── utilities/
├── tests/
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
└── requirements.txt
