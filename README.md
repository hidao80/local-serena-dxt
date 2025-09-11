# Local Serena DXT

![Claude Badge](https://img.shields.io/badge/Claude_Extension-D97757?logo=claude&logoColor=fff&style=flat)
[![License][License-Badge]][License]

## Overview

This is a Claude Desktop Extension (DXT) that allows you to launch Serena MCP in any local project and access it from the Claude Desktop app.

## Installation

1. Launch the Claude Desktop app.
2. Go to [Settings] -> [Extensions] and click the [Advanced Settings] button to open the advanced settings screen.
3. Click the [Install Extension] button. In the file selection dialog, select [local-serena.dxt] and click the [Preview] button.
4. In the preview dialog, click the [Install] button.
5. The settings dialog will open. Specify the target project and port number.
6. After closing the settings dialog, toggle the switch from [Disabled] to [Enabled] in the preview dialog. Serena MCP will start at this point.
7. Close the preview dialog.

## Usage

After launching the Claude Desktop app and enabling Local Serena DXT, Serena will start.

In this state, you can enter prompts such as "Tell me about XX in the project with Serena" in the Claude Desktop app chat. The app will operate Serena and return information.

If necessary, it will read files or write to Serena's memory files.

## Build Instructions

<details>
<summary>Steps</summary>

```sh
# Install uv and npm.
winget install astral-sh.uv OpenJS.NodeJS.LTS

# Clone this repository.
git clone https://github.com/hidao80/local-serena-dxt

# Move to the cloned local-serena directory.
cd local-serena-dxt

# Run the build script.
npm run package
```

</details>

## Directory Structure

<details>
<summary>Directory Tree</summary>

```
serena-dxt/
├── .gitignore
├── README.md     ← This file
├── README_ja.md
├── package.json
└── src/
    ├── .dxtignore
    ├── icon.png
    └── manifest.json
```

<description>
</details>

## License

MIT
