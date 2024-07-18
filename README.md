[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/XoLGRbHq)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15431489&assignment_repo_type=AssignmentRepo)
# SE-Assignment-5
Installation and Navigation of Visual Studio Code (VS Code)
 Instructions:
Answer the following questions based on your understanding of the installation and navigation of Visual Studio Code (VS Code). Provide detailed explanations and examples where appropriate.

 Questions:

1. Installation of VS Code:
   - Describe the steps to download and install Visual Studio Code on Windows 11 operating system. Include any prerequisites that might be needed.
     

 - To download and install Visual Studio Code on Windows 11, follow these steps:

 Prerequisites
1. Windows 11 operating system.
2. Administrator access to install applications.

 Step-by-Step Instructions

 Step 1: Download Visual Studio Code

1. Open your web browser and go to (https://code.visualstudio.com/).

2. Click on the "Download for Windows" button.

   (https://code.visualstudio.com/assets/docs/editor/setup/vs-code-win.png)

 Step 2: Run the Installer

1. Locate the downloaded `VSCodeSetup.exe` file (usually in your Downloads folder) and double-click it to run the installer.

   (https://code.visualstudio.com/assets/docs/editor/setup/setup-win-download.png)

2. If prompted by User Account Control, click "Yes" to allow the installer to make changes to your device.

 Step 3: Install Visual Studio Code

1. In the setup window, click "Next" to continue.

   (https://code.visualstudio.com/assets/docs/editor/setup/setup-win-welcome.png)

2. Read and accept the license agreement, then click "Next".

   (https://code.visualstudio.com/assets/docs/editor/setup/setup-win-license.png)

3. Choose the destination location for the installation (the default is usually fine), then click "Next".

   (https://code.visualstudio.com/assets/docs/editor/setup/setup-win-destination.png)

4. Select the additional tasks you want to perform while installing. It's recommended to:
   - Create a desktop icon.
   - Add "Open with Code" action to the context menu.
   - Add to PATH (this is crucial for using the `code` command in the terminal).

   After selecting your preferences, click "Next".

   (https://code.visualstudio.com/assets/docs/editor/setup/setup-win-additional-tasks.png)

5. Click "Install" to begin the installation process.

   (https://code.visualstudio.com/assets/docs/editor/setup/setup-win-ready-to-install.png)

6. Once the installation is complete, click "Finish". Ensure the "Launch Visual Studio Code" option is checked if you want to start it immediately.

   (https://code.visualstudio.com/assets/docs/editor/setup/setup-win-completed.png)

 Step 4: Launch Visual Studio Code

1. If you didn’t select the "Launch Visual Studio Code" option during the final installation step, you can start VS Code by finding it in the Start Menu or clicking the desktop icon.

2. Upon first launch, you may be prompted to customize settings or install recommended extensions.

 References
- (https://code.visualstudio.com/docs/setup/windows)

These steps will help you successfully download and install Visual Studio Code on a Windows 11 system.
  

2. First-time Setup:
   - After installing VS Code, what initial configurations and settings should be adjusted for an optimal coding environment? Mention any important settings or extensions.
  
   - After installing Visual Studio Code (VS Code), here are some initial configurations and settings to optimize your coding environment:

 1. Install Recommended Extensions

Essential Extensions
- Python: Provides rich support for the Python language.
- Prettier - Code formatter**: Formats your code consistently.
- ESLint: Integrates ESLint into VS Code for JavaScript and TypeScript.
- Live Server: Launch a development local server with a live reload feature.
- GitLens: Supercharges the built-in Git capabilities.

 How to Install Extensions
1. Click on the Extensions icon in the Activity Bar on the side of the window or press `Ctrl+Shift+X`.
2. Search for the extension name and click "Install".

(https://code.visualstudio.com/assets/docs/introvideos/extend/extensions.png)

 2. Configure Settings

 Editor Settings
1. Go to File > Preferences > Settings (or press `Ctrl+,`).
2. Adjust the following settings:

- Font Size and Family:
  ```json
  "editor.fontSize": 14,
  "editor.fontFamily": "Fira Code, Consolas, 'Courier New', monospace"
  ```

- Tab and Indentation:
  ```json
  "editor.tabSize": 2,
  "editor.insertSpaces": true
  ```

- Auto Save:
  ```json
  "files.autoSave": "afterDelay",
  "files.autoSaveDelay": 1000
  ```

- Word Wrap:
  ```json
  "editor.wordWrap": "on"
  ```

(https://code.visualstudio.com/assets/docs/getstarted/settings/JSON-config.png)

 3. Theme and Appearance

1. Go to File > Preferences > Color Theme (or press `Ctrl+K Ctrl+T`).
2. Select a theme that suits your preference. Popular choices include "Dark+ (default dark)" and "Light+ (default light)".

(https://code.visualstudio.com/assets/docs/getstarted/themes/color-theme.png)

 4. Integrate Source Control

1. Go to the Source Control icon in the Activity Bar.
2. If you have Git installed, it will be detected automatically.
3. Set up your Git user configuration:
   - Open a terminal (`Ctrl+``) and run:
     ```sh
     git config --global user.name "Your Name"
     git config --global user.email "your.email@example.com"
     ```

(https://code.visualstudio.com/assets/docs/editor/github/authentication.png)

 5. Configure Python Environment (If using Python)

1. Install the Python extension as mentioned above.
2. Select your Python interpreter:
   - Press `Ctrl+Shift+P` to open the Command Palette.
   - Type "Python: Select Interpreter" and select the appropriate interpreter from the list.

(https://code.visualstudio.com/assets/docs/python/tutorial/media/select_interpreter.png)

6. Customize Keybindings

1. Go to File > Preferences > Keyboard Shortcuts (or press `Ctrl+K Ctrl+S`).
2. Customize keybindings to fit your workflow.

(https://code.visualstudio.com/assets/docs/editor/keybindings/keybindings-editor.png)

 References
- [Visual Studio Code Documentation](https://code.visualstudio.com/docs)
- [Python in Visual Studio Code](https://code.visualstudio.com/docs/python/python-tutorial)

These configurations and settings will help you set up an optimal coding environment in VS Code.


3. User Interface Overview:
   - Explain the main components of the VS Code user interface. Identify and describe the purpose of the Activity Bar, Side Bar, Editor Group, and Status Bar.
  
   - Visual Studio Code (VS Code) has a well-organized user interface designed to enhance productivity. Here are the main components:

 1. Activity Bar
The Activity Bar is located on the far left side of the interface.

- Purpose: Provides quick access to different views and functions.
- Components:
  - Explorer: Manages files and folders.
  - Search: Allows searching across files.
  - Source Control: Integrates with version control systems like Git.
  - Run and Debug: Manages debugging configurations and controls.
  - Extensions: Accesses the marketplace to install and manage extensions.

(https://code.visualstudio.com/assets/docs/getstarted/userinterface/activity-bar.png)

 2. Side Bar
The Side Bar is located next to the Activity Bar.

- Purpose: Displays the contents of the selected Activity Bar view.
- Components:
  - Explorer: Shows file and folder structures.
  - Search Results: Displays search outcomes.
  - Source Control Changes: Lists changes in version control.
  - Run and Debug Options: Configures and starts debug sessions.
  - Installed Extensions: Lists installed extensions and their settings.

(https://code.visualstudio.com/assets/docs/getstarted/userinterface/sidebar.png)

 3. Editor Group
The Editor Group is the central area of the interface where you edit files.

- Purpose: Allows you to open and edit multiple files simultaneously.
- Components:
  - Tabs: Each open file is represented by a tab at the top of the Editor Group.
  - Split Editors: You can split the Editor Group into multiple editors side-by-side.

(https://code.visualstudio.com/assets/docs/getstarted/userinterface/editor-group.png)

 4. Status Bar
The Status Bar is located at the bottom of the interface.

- Purpose: Provides information about the current workspace and active file.
- Components:
  - Line and Column Number: Indicates the cursor's position in the active file.
  - Language Mode: Displays and changes the language mode of the file.
  - Git Branch and Sync Status: Shows the current Git branch and sync status.
  - Errors and Warnings: Displays the number of errors and warnings in the workspace.
  - Encoding, End of Line Sequence, and Indentation: Shows and allows changing file encoding, EOL sequence, and indentation settings.

(https://code.visualstudio.com/assets/docs/getstarted/userinterface/status-bar.png)

 References
- [Visual Studio Code User Interface](https://code.visualstudio.com/docs/getstarted/userinterface)

These components together provide a powerful and flexible coding environment in VS Code.


4. Command Palette:
   - What is the Command Palette in VS Code, and how can it be accessed? Provide examples of common tasks that can be performed using the Command Palette.
  
  - The Command Palette in Visual Studio Code (VS Code) is a powerful feature that provides quick access to various commands and settings without needing to navigate through menus.
 Accessing the Command Palette

You can open the Command Palette in two main ways:
1. Using the keyboard shortcut: Ctrl+Shift+P (or F1).
2. Via the menu: Go to View > Command Palette....

(https://code.visualstudio.com/assets/docs/getstarted/userinterface/command-palette.png)

 Common Tasks Performed Using the Command Palette

1. Changing the Color Theme
   - Command: Preferences: Color Theme
   - Steps: 
     1. Open the Command Palette (Ctrl+Shift+P).
     2. Type color theme.
     3. Select Preferences: Color Theme from the list.
     4. Choose a theme from the available options.

2. Installing Extensions
   - Command: Extensions: Install Extensions
   - Steps:
     1. Open the Command Palette (Ctrl+Shift+P).
     2. Type install extensions.
     3. Select Extensions: Install Extensions.
     4. Search for the desired extension and click Install.

3. Opening Settings
   - Command: Preferences: Open Settings (JSON) or Preferences: Open Settings (UI)
   - Steps:
     1. Open the Command Palette (Ctrl+Shift+P).
     2. Type settings.
     3. Select either Preferences: Open Settings (JSON) or Preferences: Open Settings (UI).

4. Running a Terminal Command
   - Command: Terminal: Create New Integrated Terminal
   - Steps:
     1. Open the Command Palette (Ctrl+Shift+P).
     2. Type create terminal.
     3. Select Terminal: Create New Integrated Terminal.

5. Git Commands
   - Command: Various Git commands like Git: Clone, Git: Commit, etc.
   - Steps:
     1. Open the Command Palette (Ctrl+Shift+P).
     2. Type git.
     3. Select the desired Git command, such as Git: Clone, Git: Commit, Git: Pull, etc.

6. Formatting a Document
   - Command: Format Document
   - Steps:
     1. Open the Command Palette (Ctrl+Shift+P).
     2. Type format document.
     3. Select Format Document to format the currently active file.

Screenshots

 Example: Changing the Color Theme
(https://code.visualstudio.com/assets/docs/getstarted/themes/color-theme.png)

 Example: Installing Extensions
(https://code.visualstudio.com/assets/docs/introvideos/extend/extensions.png)

 References
- [Visual Studio Code Documentation](https://code.visualstudio.com/docs)
- [User Interface](https://code.visualstudio.com/docs/getstarted/userinterface)

The Command Palette is a versatile tool in VS Code, allowing for efficient command execution and customization, significantly enhancing productivity.


5. Extensions in VS Code:
   - Discuss the role of extensions in VS Code. How can users find, install, and manage extensions? Provide examples of essential extensions for web development.

   - Extensions in Visual Studio Code (VS Code) enhance functionality and provide additional features to tailor the development environment to specific needs. They are crucial for adding language support, debugging tools, themes, and other utilities that improve productivity.

 Role of Extensions in VS Code
1. Language Support: Extensions add support for various programming languages, providing syntax highlighting, code completion, and debugging capabilities.
2. Tools and Utilities: Extensions offer tools like linters, formatters, debuggers, and Git integration.
3. Themes and Appearance: Extensions allow customization of the editor's appearance with different themes and icon packs.
4. Framework and Library Support: Extensions add specific support for frameworks like React, Angular, Vue.js, etc.

 Finding, Installing, and Managing Extensions
 
 Finding Extensions

 1. Via the Extensions View:
   - Click on the Extensions icon in the Activity Bar on the side of the window.
   - Use the search bar to find specific extensions.

   (https://code.visualstudio.com/assets/docs/introvideos/extend/extensions.png)

2. Via the Command Palette:
   - Open the Command Palette (`Ctrl+Shift+P`).
   - Type `Extensions: Install Extensions`.

   (https://code.visualstudio.com/assets/docs/getstarted/userinterface/command-palette.png)

 Installing Extensions

1. From the Extensions View:
   - Find the desired extension using the search bar.
   - Click on the `Install` button next to the extension.

   (https://code.visualstudio.com/assets/docs/introvideos/extend/install.png)

2. From the Marketplace Website:
   - Go to the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/vscode).
   - Search for the extension and click on `Install`.

 Managing Extensions

1. View Installed Extensions:
   - Go to the Extensions View.
   - Installed extensions are listed at the top.

2. Disable/Enable Extensions:
   - Click on the gear icon next to an installed extension.
   - Select `Disable` or `Enable`.

3. Uninstall Extensions:
   - Click on the gear icon next to an installed extension.
   - Select `Uninstall`.

   (https://code.visualstudio.com/assets/docs/introvideos/extend/manage.png)

 Essential Extensions for Web Development

1. ESLint
   - Purpose: Integrates ESLint into VS Code for identifying and fixing linting errors in JavaScript and TypeScript.
   - Installation: Search for `ESLint` in the Extensions View and click `Install`.

2. Prettier - Code formatter
   -Purpose: Automatically formats code to ensure consistency.
   - Installation: Search for `Prettier - Code formatter` and click `Install`.

3. Live Server
   - Purpose: Launches a local development server with live reload feature for static and dynamic pages.
   - Installation: Search for `Live Server` and click `Install`.

4. Bracket Pair Colorizer 2
   - Purpose: Adds different colors to matching brackets to improve code readability.
   - Installation: Search for `Bracket Pair Colorizer 2` and click `Install`.

5. Path Intellisense
   - **Purpose: Provides autocomplete for file paths in the project.
   - Installation: Search for `Path Intellisense` and click `Install`.

6. GitLens
   - **Purpose: Enhances Git capabilities in VS Code, providing detailed history and blame information.
   - Installation: Search for `GitLens` and click `Install`.

Screenshots

Example: Installing ESLint
(https://code.visualstudio.com/assets/docs/introvideos/extend/install-eslint.png)

 References
- [Visual Studio Code Documentation](https://code.visualstudio.com/docs)
- [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/vscode)

Extensions play a crucial role in customizing and enhancing the functionality of VS Code, making it a powerful tool for web development and other programming tasks.



6. Integrated Terminal:
   - Describe how to open and use the integrated terminal in VS Code. What are the advantages of using the integrated terminal compared to an external terminal?
     
  
   -  Opening and Using the Integrated Terminal in VS Code

The integrated terminal in Visual Studio Code (VS Code) allows you to run shell commands directly within the editor, providing a seamless workflow for development tasks.

 Steps to Open the Integrated Terminal

1. Using the Menu:
   - Go to the top menu and select `View` > `Terminal`.

2. Using the Keyboard Shortcut:
   - Press `Ctrl+` (backtick) or `Ctrl+Shift+` (backtick) to open the terminal.

   (https://code.visualstudio.com/assets/docs/editor/integrated-terminal/terminal-menu.png)

3. Using the Command Palette:
   - Open the Command Palette by pressing `Ctrl+Shift+P`.
   - Type `Toggle Integrated Terminal` and select it.

   (https://code.visualstudio.com/assets/docs/getstarted/userinterface/command-palette.png)

 Using the Integrated Terminal

1. Running Commands:
   - Type commands as you would in any other terminal. For example, you can run `git status`, `npm install`, or `python script.py`.

   (https://code.visualstudio.com/assets/docs/editor/integrated-terminal/running-commands.png)

2. Creating Multiple Terminals:
   - Click the `+` icon in the terminal panel to open a new terminal.
   - Use the dropdown menu next to the `+` icon to switch between different terminals.

   (https://code.visualstudio.com/assets/docs/editor/integrated-terminal/multiple-terminals.png)

3. Splitting the Terminal:
   - Click the split terminal button to divide the current terminal into two.

   (https://code.visualstudio.com/assets/docs/editor/integrated-terminal/split-terminal.png)

4. Customizing Terminal Settings:
   - You can customize the terminal's appearance and behavior via the settings (`Ctrl+,`).
   - For example, you can change the font size, terminal shell, or colors.

   (https://code.visualstudio.com/assets/docs/editor/integrated-terminal/customize-terminal.png)

 Advantages of Using the Integrated Terminal

1. Seamless Workflow:
   - Allows for efficient context switching between code and terminal commands, reducing disruption in the development workflow.

2. Environment Consistency:
   - Ensures the terminal environment matches the VS Code workspace settings, providing consistency across different development tasks.

3. Convenience:
   - Eliminates the need to switch between different applications, streamlining the development process.

4. Panel Integration:
   - The terminal is docked within the VS Code interface, providing easy access to terminal output and code simultaneously.

5. Customization:
   - Offers extensive customization options for the terminal, including themes, shell integration, and keybindings.

6. Multi-terminal Management:
   - Supports multiple terminal instances and split terminals, making it easier to manage various tasks and commands within the same interface.

References
- [Visual Studio Code Integrated Terminal Documentation](https://code.visualstudio.com/docs/editor/integrated-terminal)

The integrated terminal in VS Code enhances productivity by providing a powerful, customizable, and convenient terminal experience within the editor itself.



7. File and Folder Management:
   - Explain how to create, open, and manage files and folders in VS Code. How can users navigate between different files and directories efficiently?
  
   - Creating, Opening, and Managing Files and Folders in VS Code

 Creating Files and Folders

1. Using the Explorer View:
   - Click on the Explorer icon in the Activity Bar (or press `Ctrl+Shift+E`).
   - Right-click on the folder where you want to create the file or folder.
   - Select `New File` or `New Folder`.
   - Enter the desired name and press `Enter`.

   (https://code.visualstudio.com/assets/docs/editor/codebasics/create-file-folder.png)

2. Using the Command Palette:
   - Open the Command Palette (`Ctrl+Shift+P`).
   - Type `File: New File` or `File: New Folder` and select the respective command.
   - Enter the name and press `Enter`.

   (https://code.visualstudio.com/assets/docs/getstarted/userinterface/command-palette.png)

 Opening Files and Folders

1. Using the Explorer View:
   - Navigate to the file or folder in the Explorer.
   - Double-click on a file to open it.

   (https://code.visualstudio.com/assets/docs/editor/codebasics/open-file-explorer.png)

2. Using the Command Palette:
   - Open the Command Palette (`Ctrl+Shift+P`).
   - Type `File: Open File` and select it.
   - Navigate to the file you want to open and press `Enter`.

   (https://code.visualstudio.com/assets/docs/getstarted/userinterface/command-palette.png)

 Managing Files and Folders

1. Renaming:
   - Right-click on a file or folder in the Explorer.
   - Select `Rename` from the context menu.
   - Enter the new name and press `Enter`.

   (https://code.visualstudio.com/assets/docs/editor/codebasics/rename-file.png)

2. Deleting:
   - Right-click on a file or folder in the Explorer.
   - Select `Delete` from the context menu.
   - Confirm the deletion.

   (https://code.visualstudio.com/assets/docs/editor/codebasics/delete-file.png)

3. Moving:
   - Drag and drop files or folders within the Explorer view to move them to a different location.

   (https://code.visualstudio.com/assets/docs/editor/codebasics/move-file.png)

Navigating Between Files and Directories Efficiently

1. Quick Open:
   - Press `Ctrl+P` to open the Quick Open dialog.
   - Start typing the name of the file you want to open.
   - Select the file from the filtered list and press `Enter`.

   (https://code.visualstudio.com/assets/docs/getstarted/userinterface/quick-open.png)

2. Go to File:
   - Open the Command Palette (`Ctrl+Shift+P`).
   - Type `Go to File...` and select it.
   - Start typing the name of the file and press `Enter` to open it.

   (https://code.visualstudio.com/assets/docs/getstarted/userinterface/command-palette.png)

3. Explorer View Navigation:
   - Expand and collapse folders in the Explorer view to navigate through the directory structure.
   - Use the breadcrumb navigation at the top of the editor to quickly switch between parent folders.

   (https://code.visualstudio.com/assets/docs/editor/codebasics/explorer-navigation.png)

 References
- [Visual Studio Code Documentation](https://code.visualstudio.com/docs)
- [Code Editing in Visual Studio Code](https://code.visualstudio.com/docs/editor/codebasics)

By utilizing these methods, users can effectively create, open, manage files and folders, and navigate between different files and directories efficiently within Visual Studio Code.



8. Settings and Preferences:
   - Where can users find and customize settings in VS Code? Provide examples of how to change the theme, font size, and keybindings.
  
   - ### Finding and Customizing Settings in VS Code

In Visual Studio Code (VS Code), users can find and customize settings through the Settings UI, JSON settings file, and the Command Palette. Here’s how to locate and customize settings for changing the theme, font size, and keybindings:

#### 1. **Settings UI**

- **Accessing Settings**:
  - Click on the gear icon (`⚙️`) in the lower-left corner of the VS Code window and select `Settings`.
  - Alternatively, press `Ctrl+,` (comma) to open the Settings UI directly.

  ![Settings UI](https://code.visualstudio.com/assets/docs/getstarted/settings/settings-icon.png)

- **Changing the Theme**:
  1. In the Settings UI, type "theme" in the search box.
  2. Click on the `Color Theme` dropdown and select a theme from the list.

  ![Change Theme](https://code.visualstudio.com/assets/docs/getstarted/themes/select-color-theme.png)

- **Adjusting Font Size**:
  1. In the Settings UI, type "font size" in the search box.
  2. Use the `Editor: Font Size` setting to adjust the font size as desired.

  ![Adjust Font Size](https://code.visualstudio.com/assets/docs/getstarted/settings/font-size.png)

- **Customizing Keybindings**:
  1. In the Settings UI, type "keybindings" in the search box.
  2. Click on `Open Keyboard Shortcuts (JSON)` to edit keybindings directly in the `keybindings.json` file.

  ![Customize Keybindings](https://code.visualstudio.com/assets/docs/getstarted/keybindings/keybindings-json.png)

#### 2. **JSON Settings File**

- **Accessing JSON Settings**:
  - Click on the `Open Settings (JSON)` link at the top right of the Settings UI to directly edit the `settings.json` file.

  ![Open Settings JSON](https://code.visualstudio.com/assets/docs/getstarted/settings/open-settings-json.png)

- **Example: Changing the Theme in `settings.json`**:
  ```json
  "workbench.colorTheme": "Default Dark+"
  ```

- **Example: Adjusting Font Size in `settings.json`**:
  ```json
  "editor.fontSize": 14
  ```

- **Example: Customizing Keybindings in `keybindings.json`**:
  ```json
  // Example keybinding for commenting code
  {
      "key": "ctrl+/",
      "command": "editor.action.commentLine",
      "when": "editorTextFocus && !editorReadonly"
  }
  ```

#### 3. **Command Palette**

- **Accessing Settings via Command Palette**:
  - Open the Command Palette (`Ctrl+Shift+P`).
  - Type specific settings commands like `Preferences: Color Theme`, `Preferences: Open Settings (JSON)`, or `Preferences: Open Keyboard Shortcuts (JSON)`.

### Examples and Screenshots

- **Changing Theme**:
  ![Change Theme Example](https://code.visualstudio.com/assets/docs/getstarted/themes/select-color-theme.png)

- **Adjusting Font Size**:
  ![Adjust Font Size Example](https://code.visualstudio.com/assets/docs/getstarted/settings/font-size.png)

- **Customizing Keybindings**:
  ![Customize Keybindings Example](https://code.visualstudio.com/assets/docs/getstarted/keybindings/keybindings-json.png)

### References
- [Visual Studio Code Documentation - Settings](https://code.visualstudio.com/docs/getstarted/settings)
- [Visual Studio Code Documentation - Keybindings](https://code.visualstudio.com/docs/getstarted/keybindings)

Customizing settings in VS Code using these methods allows users to personalize their coding environment effectively, improving productivity and comfort during development tasks.
  
9. 

10. Debugging in VS Code:
   - Outline the steps to set up and start debugging a simple program in VS Code. What are some key debugging features available in VS Code?

11. Using Source Control:
    - How can users integrate Git with VS Code for version control? Describe the process of initializing a repository, making commits, and pushing changes to GitHub.

 Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide screenshots or step-by-step instructions where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by 1st July 

