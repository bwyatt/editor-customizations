# Editor Customizations

Personal GitHub Copilot customization files for use across my development environments. This repository is intended to be added to Copilot settings in VS Code (instructions below) for use in all repos.

## Usage

1. Clone this repository to your machine.
2. In VS Code, add the following paths to their respective settings:
   - **Prompt files** — Add the `.github/prompts` folder to the [Chat: Prompt Files Locations](vscode://settings/chat.promptFilesLocations) setting (e.g. `~/Git/editor-customizations/.github/prompts`).
   - **Instruction files** — Add the `.github/instructions` folder to the [Chat: Instruction Files Locations](vscode://settings/chat.instructionsFilesLocations) setting (e.g. `~/Git/editor-customizations/.github/instructions`).

The reusable prompts and instruction files will then be available in Copilot Chat across all your workspaces. The `copilot-instructions.md` file is picked up automatically when this repository is open in VS Code.

Per-repository instruction files take precedence over the instructions defined here. If there are conflicts, Copilot will ask for clarification.

## Contents

### Copilot Instructions

[`.github/copilot-instructions.md`](.github/copilot-instructions.md) — Global instructions that guide Copilot's behavior across all coding tasks. Covers coding principles such as prioritizing correctness and readability, handling edge cases, and following project conventions.

### Reusable Prompts

Located in `.github/prompts/`:

| Prompt | Description |
|--------|-------------|
| [`codereview.prompt.md`](.github/prompts/codereview.prompt.md) | Conducts a thorough code review of branch changes, covering quality, functionality, testing, security, and more. |
| [`debug.prompt.md`](.github/prompts/debug.prompt.md) | Investigates an issue in the codebase, identifies potential causes, and proposes resolution plans. |
| [`featureplan.prompt.md`](.github/prompts/featureplan.prompt.md) | Develops a detailed implementation plan for a new feature before any code is written. |
