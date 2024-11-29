# Remote Desktop Developer Guide

## Introduction

[Remote Desktop]() is an Electron-based graphical user interface for Scrcpy, designed to facilitate the display and control of Android devices

## Getting Started

### System Requirements
- Node.js v20 or higher


### Development Setup

# Enable pnpm package manager
corepack enable pnpm

# Install dependencies
pnpm install

# Start development server
pnpm dev

# Build applications
pnpm build          # Auto-detect platform
pnpm build:win      # Build for Windows
pnpm build:mac      # Build for macOS 
pnpm build:linux    # Build for Linux
```

## Technical Architecture

### Core Technologies
- Electron - Cross-platform desktop application framework
- Vue.js - Frontend framework
- JavaScript - Primary programming language
- Node.js - Runtime environment
- scrcpy - Android device display and control
- adbkit - Android Debug Bridge toolkit

### Project Structure
```
📦Remote Desktop
 ┣ 📂.vscode             # VSCode editor settings
 ┣ 📂control             # Device floating control bar
 ┣ 📂electron          # Electron main process
 ┣ 📂src               # Main renderer process
 ┃ ┣ 📂assets         # Static resources
 ┃ ┣ 📂components     # Vue components
 ┃ ┃ ┣ 📂Device      # Device management
 ┃ ┃ ┣ 📂Preference  # Settings interface
 ┃ ┃ ┗ 📂Quick       # Quick access features
 ┃ ┣ 📂composables   # Vue composition functions
 ┃ ┣ 📂configs       # App configurations
 ┃ ┣ 📂dicts         # Constants and enums
 ┃ ┣ 📂icons         # Icon assets
 ┃ ┣ 📂locales       # Internationalization
 ┃ ┣ 📂plugins       # Vue plugins
 ┃ ┣ 📂store         # State management
 ┃ ┣ 📂styles        # Global styles
 ┃ ┗ 📂utils         # Helper functions
 ┣ 📂public             # Public assets
 ┣ 📂screenshots        # Application screenshots
 ┣ 📂scripts           # Build scripts
 ┣ 📜.eslintrc-auto-import.json  # ESLint settings
 ┣ 📜package.json      # Project metadata
 ┣ 📜vite.config.js    # Build configuration
 ┗ 📜electron-builder.json  # Electron packaging config
```

## Reference Documentation

- [Electron](https://www.electronjs.org/docs)
- [Vue.js](https://vuejs.org/)
- [Scrcpy](https://github.com/Genymobile/scrcpy)
- [Adbkit](https://github.com/DeviceFarmer/adbkit)