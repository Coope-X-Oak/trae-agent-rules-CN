# Trae Agent Rules (Learning Edition)

[中文](README.md) | **English**

This is a learning project about Trae IDE agent rule configuration, aiming to improve the efficiency and accuracy of AI-assisted programming through standardized and structured rule definitions.

## ⚠️ Disclaimer

This project is a learning work by me ([@Cooper-X-Oak](https://github.com/Cooper-X-Oak/)). The content is deeply inspired by Agent Rules related projects in the open-source community, and has been refactored, localized, and customized to fit the Trae IDE workflow.

## ✨ Highlights

This project has undergone deep standardization and structural transformation of Agent Rules. Key features include:

1.  **Self-Referential Evolution**
    *   **Core Philosophy**: This project builds a "self-referential" documentation system, meaning it uses the rule system itself to regulate and improve rule creation.
    *   **Extreme Minimalism**: Adopts `Key:Value` format, discarding verbose descriptions to maximize Token utilization.
    *   **Strong Constraint Directives**: Uses keywords like `MUST`, `NEVER`, `REQUIRED` to reduce ambiguity.

2.  **Smart Triggering**
    *   **`alwaysApply: true`**: Globally effective (e.g., Language Constraint).
    *   **`globs: "*.md"`**: Automatically triggered based on file paths.
    *   **`description: "..."`**: Intelligently triggered based on semantic context.

3.  **Standardized Categories**
    *   All rule files follow the `Category-FeatureName.md` format with clear classification (Global/Core/Docs/Tech/Tools).

## 📂 Directory Structure

All rule files are located in the `TRAERULES_EN/` directory (for English version), managed in a flat structure:

*   **`RULEOFRULES.md`**: **[Core Meta-Rule]** Defines the constitutional standards that all rules must follow.
*   **Core**
    *   `Core-LanguageConstraint.md`: Global language constraint (Enforces English).
    *   `Core-BugFixExpert.md`: Standardized Bug fix process.
    *   `Core-TechImplementationArchitect.md`: Code implementation and architecture design.
    *   ... (Comprehensive Review, Root Cause Analysis, etc.)
*   **Docs**
    *   `Docs-ReadmeMaintainer.md`: Maintains project entry documentation.
    *   `Docs-TechWriter.md`: Writes technical documentation.
    *   ... (Changelog, Context Guide, etc.)
*   **Tech**
    *   `Tech-ModernSwiftExpert.md`: Swift development standards.
    *   `Tech-BrowserAutomationEng.md`: Browser automation development.
*   **Tools**
    *   `Tools-GithubProjectManager.md`: Github project management.
    *   `Tools-GitCommitExpert.md`: Standardized Git commits.
    *   ... (MCP Config, System Visualization, etc.)

## 🚀 Usage

This repository only contains the organized rule files and **does not include** Trae's project configuration or raw materials.

### 1. Get Rules
```bash
git clone https://github.com/Cooper-X-Oak/trae-agent-rules-CN.git
```

### 2. Integrate into Project
1.  In your Trae project root directory, create a `.trae/rules/` folder.
2.  Copy all `.md` files from the `TRAERULES_EN` folder to the `.trae/rules/` directory.
3.  **Important**: Ensure `RULEOFRULES.md` and `Core-LanguageConstraint.md` are included to guarantee the basic experience.

### 3. Verify
Open any file or start a conversation in Trae. The AI will automatically load the corresponding rules based on the current context (file type or your question).

## 🤝 Contributing

Issues and Pull Requests are welcome to improve the rule library!

1.  Fork this repository.
2.  Create a feature branch (`git checkout -b feature/AmazingRule`).
3.  Write a new rule following the standard in `RULEOFRULES.md`.
4.  Commit changes (`git commit -m 'feat: Add AmazingRule'`).
5.  Push to branch (`git push origin feature/AmazingRule`).
6.  Submit a Pull Request.

## 📄 License

[MIT License](LICENSE)

---
*Created with ❤️ by Cooper-X-Oak using Trae IDE*
