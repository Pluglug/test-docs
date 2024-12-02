早速ドキュメントの構想にうつります。
Blenderアドオン Pie Menu Editorのドキュメントを作成中です。
まずは現在の構成からPMEの全容を理解してください。
優れた構成にするためのアドバイスをお願いします。


# Getting Started
## About Pie Menu Editor
## Installation
## Version Compatibility
  - Support for Blender 4.0+
    関連: FAQ: How to Apply Patches
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
Hotkeysを押したとき、または離したときに異なる動作を設定できます。一時的にツールやモードを有効化する際に便利です。
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
(Advanced Settingsは各エディターごとに存在するが、Pollは共通のもので重要な要素)

## UI Customization
### Panel Group (Side Panel Editor)
Allows to create a group of panels and add it to the new or existing category (tab).
### Hiding Unused Panels
The editor allows to hide a group of panels.
### PME Toolbars (Pop-up Dialog Editor)
BlenderのPreference Editorの領域を一定まで狭めると表示され、カスタムボタンを配置できる。Popup Daialogのメニュー名が” Toolbar Layout Left”などのときに識別される。
### Menu/Panel Extension (Pop-up Dialog Editor/Regular Menu Editor)
Blenderの任意のパネル/メニューにPMEアイテムをappend prependする。PME itemのメニュー名が” USERPREF_HT_header”などIDのときに識別される。
関連: Interactive Panels Mode

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
    info areaやコンソールで積極的にログを取得する
 - Interactive Panels Mode
    BlenderのすべてのUI要素にPME Toolsボタンが追加され、メニューIDを取得したりExtending Panelsなどを簡単に設定できる。
## Custom icon
pie_menu_editor/iconにアイコン画像を格納しておくとPME内でカスタムアイコンとして利用できる
## Auto Run
pie_menu_editor/scripts/auto_runにスクリプトを格納すると、PME起動時に自動で実行される

---

# Reference
## Terminology
## PME Scripting Reference
### Global Variables
### Built-in Functions
  <!-- - Property Types -->
  <!-- - Event System -->
  <!-- - Context System -->

---

# Scripting Guide
## Blender Basics
  - Understanding Blender's UI
  - Data Structure
  - Operator System
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

生成AIを使用した例

- Script Collection
    - Installation Guide
    - Available Scripts
    - Usage Instructions
    - Contributing Guidelines
- Knowledge Base
    - Tips & Tricks
    - Problem Solving
    - Performance Tips
    - Known Limitations


<!-- 
# Library (Advanced Resources)
- Glossary
- Scripting Reference
    - Global Variables
    - Built-in Functions
- Community Scripts
    - How to Use Scripts
    - Script Library
- Code Examples
    - Menu Creation
    - Custom Operations
    - Event Processing
- PMEを高度に使いこなすためのガイド
    - 前書き
    - Hotkeyを適切なKeymapに設定する
    - Pollを使用する
    - Introduction to Scripting
        - Basic knowledge of Blender
        - Basic Python
            Pythonの基本やPMEで頻繁に使用する必要のある三項演算子やリスト内包表記をあつかう
        - How to use bpy
            高度なカスタマイズをするためのBlenderのcontext, data, ops, area, UIlayoutなどについての説明
    - Practical Examples
-->

---

# Support & Community
- Get Support
- Frequently Asked Questions
    How to Apply Patches
- Known Issues
- Contribute to PME
    Bug Reporting
    Script Sharing
    (Hot!)ドキュメントの共同編集者募集(Githubなどでの貢献方法)
        Translation Help
- Changelog
