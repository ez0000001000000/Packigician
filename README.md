# Packigician 🧙‍♂️

A simple CLI tool that generates npm package templates with placeholder files you can edit.

## Installation

```bash
npm install -g packigician
```

## Usage

Create a new package template:

```bash
packigician-create my-package-name
```

Or use default name:

```bash
packigician-create
```

This creates a folder with template files containing placeholders you can edit:

### 📦 Generated Files

```
my-package-name/
├── package.json          # Template with placeholders
├── index.js             # Main entry point template
├── README.md            # Documentation template
├── .gitignore          # Git ignore file
└── bin/
    └── cli.js          # CLI command template
```

### 🎯 What You Get

**package.json** with placeholders:
- `YOUR_PACKAGE_NAME` - Replace with your package name
- `YOUR_PACKAGE_DESCRIPTION` - Replace with description
- `YOUR_NAME` - Replace with your name
- `YOUR_USERNAME` - Replace with GitHub username
- `YOUR_CLI_COMMAND` - Replace with your CLI command name

**bin/cli.js** with placeholders:
- Ready-to-use CLI structure with Commander.js
- TODO comments showing where to add your commands
- Placeholder text you can replace

**index.js** with placeholders:
- Basic module export structure
- TODO comments for your functionality

**README.md** with placeholders:
- Template documentation
- Installation and usage examples
- Placeholder text to customize

### ⚡ Features

- **No questions asked** - Just creates files
- **Template placeholders** - Easy to find and replace
- **Auto npm install** - Dependencies installed automatically
- **Professional structure** - Follows npm best practices
- **CLI ready** - Includes CLI command setup

### 📝 Quick Start

```bash
# Create package
packigician-create my-awesome-tool

# Edit files
cd my-awesome-tool
# Edit package.json, bin/cli.js, index.js, README.md

# Test your CLI
npm start hello

# Publish when ready
npm publish
```

## Requirements

- Node.js >= 14.0.0
- npm for package management

## Development

To install locally for development:

```bash
npm link
```

Then test:

```bash
packigician-create test-package
```

## License

MIT