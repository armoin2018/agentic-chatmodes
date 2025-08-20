# Agentic Chatmodes for GitHub Copilot

This repository contains custom chatmodes for GitHub Copilot.

## How to Install Custom Chatmodes

Follow these steps to install and use the custom chatmodes from this repository.

### 1. Clone the Repository

First, you need to clone this repository to your local machine.

```sh
git clone https://github.com/armoin2018/agentic-chatmodes.git
cd agentic-chatmodes
```

### 2. Locate Your GitHub Copilot Extension Directory

The location of the Copilot extension directory varies depending on your editor:

*   **Visual Studio Code:**
    `~/.vscode/extensions/github.copilot-*`
*   **JetBrains IDEs (IntelliJ, PyCharm, etc.):**
    `~/Library/Application Support/JetBrains/<Your_IDE_Name>/plugins/github-copilot`

Navigate to the directory that contains the highest version number if you have multiple `github.copilot-*` folders.

### 3. Copy the Chatmode Files

Copy the `.chatmode.md` files from this repository into a `chatmodes` directory inside your Copilot extension folder. If the `chatmodes` directory does not exist, you will need to create it.

```sh
# Example for VS Code
mkdir -p ~/.vscode/extensions/github.copilot-*/chatmodes
cp .github/chatmodes/*.chatmode.md ~/.vscode/extensions/github.copilot-*/chatmodes/
```
*Note: Replace `github.copilot-*` with the specific version of the extension you have installed.*

### 4. Restart Your Editor

For the changes to take effect, you must restart your editor (e.g., close and reopen Visual Studio Code).

### 5. Select the Chatmode

Once your editor has restarted, you can select the new chatmode in the GitHub Copilot chat panel. Look for a dropdown menu or settings option within the chat interface to switch between available chatmodes.

---

## Contributing

If you have ideas for new chatmodes or improvements to existing ones, feel free to open an issue or submit a pull request.

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/your-chatmode-name`).
3.  Add your new `.chatmode.md` file to the `.github/chatmodes/` directory.
4.  Commit your changes (`git commit -m 'Add some great new chatmode'`).
5.  Push to the branch (`git push origin feature/your-chatmode-name`).
6.  Open a pull request.

Enjoy your enhanced chat experience with GitHub Copilot!
