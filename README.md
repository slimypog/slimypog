# Slayers Unleashed II
  **Slayers Unleashed II** is a sequel to [Slayers Unleashed](https://www.roblox.com/games/6536647319/), a Demon Slayer-inspired Roblox RPG game. The GDD for this project can be found [here](https://docs.google.com/document/d/1WdsdEWrbrlV6OHICpyzLFNyIVL65h9dqeYnPTooB_OE/edit?usp=sharing).

## Developer Tools
If you are setting up this repository for the first time, you may hae to install these tools:
- [Visual Studio Code](https://code.visualstudio.com/) <br> _Extensions:_
  - [roblox-ts](https://marketplace.visualstudio.com/items?itemName=Roblox-TS.vscode-roblox-ts) _- roblox typescript support_
  - [Flamework](https://marketplace.visualstudio.com/items?itemName=flamework.flamework-vscode) _- dependency injection & metadata tags_
  - [Rojo](https://marketplace.visualstudio.com/items?itemName=evaera.vscode-rojo) _- roblox studio sync_
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) _- static code analysis_
  - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) _- opinionated code formatting_
  - [Zap_Nax](https://marketplace.visualstudio.com/items?itemName=naxblox.zap-nax) _- optional, syntax highlighting for .zap files_
- [Git SCM](https://git-scm.com/)
- [Aftman](https://github.com/LPGhatguy/aftman) _(you must restart your device after installing this)_
- [Node.js v20](https://nodejs.org/en/download)

## Useful Guides & Documentation
- [Lua 5.1](https://www.lua.org/manual/5.1/) _- Upstream version of Lua that Luau is based on_
- [Luau](https://luau-lang.org/getting-started) _- Superset of Lua 5.1 used by Roblox_
- [TypeScript](https://www.typescriptlang.org/docs/) _- Statically-typed, open-source, high-level programming language by Microsoft_
- [roblox-ts](https://roblox-ts.com/docs/) _- Compiles TypeScript code into Luau code_
- [Flamework](https://flamework.fireboltofdeath.dev/docs/introduction) _- Extensible game framework including decorators for services, controllers, and components_
- [Reflex](https://littensy.github.io/reflex/docs/guides/your-first-producer) _- Immutable state container_
- [React JS](https://react.dev/learn) _- Declarative, component-based user interface library in JS_
- [React Lua](https://jsdotlua.github.io/react-lua/) _- React translated to Lua_
- [Ripple](https://github.com/littensy/ripple#readme) _- Motion/animation library for React Lua_
- [Beacon](https://github.com/Sleitnick/rbxts-beacon#readme) _- Event signal library_
- [GameJoy](https://github.com/Rimuy/GameJoy#readme) _- Class-based user input library_
- [Octo-Tree](https://github.com/Sleitnick/rbxts-octo-tree#readme) _- Octree library_

## Getting Started
### Setting up Git
#### Set your Git Username & Email
  - At the top of the VSC window, go to Terminal -> New Terminal
  - Type `git config --global user.name "GitHub Username"` in the Terminal, replacing "GitHub Username" with your GitHub username, then press Enter
  - Type `git config --global user.email "GitHub Email"` in the Terminal, replacing "GitHub Email" with the email associated with your GitHub account, then press Enter

#### Clone the Git Repository
  - Create a new folder somewhere on your file system for git repositories if you haven't already; it's suggested to put this folder inside your "Documents" folder and give it a name without spaces like "Git-Repositories"
  - Open a "Git Bash" window
  - Type `cd C:/path/to/your/folder` in Git Bash, replacing "C:/path/to/your/folder" with the path to the folder you created in the previous step, then press Enter
  - Type `git clone https://github.com/Credenzio-Studios/Slayers-Unleashed-II.git` in Git Bash, then press Enter
  - Wait for git clone to finish, it may take a long time depending on your network/internet speed

---
### Setting up Visual Studio Code
_Note: If at any point after launching VSC you get a notification asking whether you want to periodically run `git fetch`, choose "Yes"_
#### Set Integrated Terminal to Git Bash
  - At the top left of the VSC window, go to File -> Preferences -> Settings
  - In the search bar at the top, type in `terminal.integrated.defaultProfile.windows`
  - Set the "Terminal > Integrated > Default Profile > Windows" option to "Git Bash"
  - Press CTRL + S to save your settings

#### Open the Git Repository in VSC
  - At the top left of the VSC window, go to File -> Open Folder
  - Navigate to the location of your folder for this repository, select it and press "Select Folder"

#### Install Dependencies
  - At the top of the VSC window, go to Terminal -> New Terminal
  - Type `aftman install` in the Terminal, then press Enter
    - If you are prompted to give permission to install tools, type Y and press Enter for each one
  - Type `npm install` in the Terminal, then press Enter

#### Set up Rojo in VSC
  - In VSC, press CTRL + SHIFT + P to open the Command Palette
  - Type `>rojo` in the Command Palette search bar
  - Click on "Rojo: Open Menu"
  - Click on "Install Roblox Studio Plugin"

---
### Workflow
#### Using Roblox-TS Compiler
  - At the bottom right of the VSC window, press the "▷ roblox-ts" button
    - After pressing the button, Roblox-TS will start watching for file changes and recompile to the "./out/" folder any time a file is changed _(can run at the same time as Rojo, it should not conflict)_
    - Pressing the button again will stop the compiler

#### Using Rojo
  - At the bottom right of the VSC window, press the "🚀 Rojo" button
    - After pressing the button, Rojo will start a local web server on your device to communicate with the Roblox Studio plugin
    - Pressing the button again will stop the local web server
  - To sync into Roblox Studio, find the Rojo plugin in your Roblox Studio and hit "Connect"
