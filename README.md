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

### Instruction Files

Located in `.github/instructions/`:

| File | Applies To | Description |
|------|-----------|-------------|
| [`code-review.instructions.md`](.github/instructions/code-review.instructions.md) | `**` | Generic code review instructions that can be customized for any project using GitHub Copilot. |
| [`feature-planning.instructions.md`](.github/instructions/feature-planning.instructions.md) | `**` | Guidelines for planning new features with structured design documents and implementation plans. |
| [`instructions.instructions.md`](.github/instructions/instructions.instructions.md) | `**/*.instructions.md` | Guidelines for creating high-quality custom instruction files for GitHub Copilot. |
| [`prompt.instructions.md`](.github/instructions/prompt.instructions.md) | `**/*.prompt.md` | Guidelines for creating high-quality prompt files for GitHub Copilot. |

### Reusable Prompts

Located in `.github/prompts/`:

| Prompt | Description |
|--------|-------------|
| [`debug.prompt.md`](.github/prompts/debug.prompt.md) | Investigates an issue in the codebase, identifies potential causes, and proposes resolution plans. |
