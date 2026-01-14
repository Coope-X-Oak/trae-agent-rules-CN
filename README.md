# Trae Agent Rules (Learning Edition)

这是一个关于 Trae IDE 智能体规则配置的学习项目。简单来说，我正在尝试通过一套标准化、结构化的规则定义，让 AI 辅助编程变得更聪明、更顺手。

## ⚠️ 声明 (Disclaimer)

本项目是我 ([@Cooper-X-Oak](https://github.com/Cooper-X-Oak/)) 的学习之作。内容深受开源社区 Agent Rules 相关项目的启发，我在此基础上稍微折腾了一下——进行了重构、汉化和定制，主要是为了更好地适应 Trae IDE 的工作流。

## ✨ 项目亮点 (Highlights)

我对 Agent Rules 做了一些深度的改造，其中最核心的哲学是：

1.  **自我指向的递归进化 (Self-Referential Evolution)**
    *   **这事儿挺有意思的**：我正在构建一个“自我指向”的文档系统。简单说，就是**我正在利用这套规则系统来纠正和完善这套规则系统本身**。
    *   就像是编程里的“自举” (Bootstrapping)，我定义的规则（比如 `RULEOFRULES`）反过来约束我如何编写新的规则。这不仅仅是一堆死板的文档，而是一个正在尝试自我完善的“规则生命体”。
    *   当然，落实到细节上，我们依然保持了**极致精简**：
        *   **Token 能省则省**：全用 `Key:Value` 键值对，摒弃那些花里胡哨的长篇大论。
        *   **有话直说**：`MUST`, `NEVER` 直接怼上去，减少歧义，AI 听了都说好。

2.  **更聪明的生效模式 (Smart Triggering)**
    *   **`alwaysApply: true`**: 全局都管用（比如那个必须讲中文的规范）。
    *   **`globs: "*.md"`**: 看到特定文件才激活，不该管的时候绝不插手。
    *   **`description: "..."`**: 只有你聊到相关话题（比如修Bug）时，专家才会现身。

3.  **治愈强迫症的分类 (Standardized Categories)**
    *   所有文件都按 `Category-功能名称.md` 排好了，Global/Core/Docs/Tech/Tools 分得清清楚楚，看着就舒服。

## 📂 目录结构

所有规则文件均位于 `TRAERULES/` 目录下，扁平化管理：

*   **`RULEOFRULES.md`**: **[核心元规则]** 定义了所有规则必须遵循的宪法级标准。
*   **Core (核心类)**
    *   `Core-中文交互规范.md`: 全局语言约束，确保中文回复。
    *   `Core-Bug修复专家.md`: 标准化 Bug 修复流程。
    *   `Core-技术实现架构师.md`: 代码实现与架构设计。
    *   ... (全视角审查、根因分析等)
*   **Docs (文档类)**
    *   `Docs-Readme管理员.md`: 维护项目入口文档。
    *   `Docs-技术文档工程师.md`: 编写技术文档。
    *   ... (版本日志、上下文引导等)
*   **Tech (技术栈类)**
    *   `Tech-现代Swift专家.md`: Swift 开发规范。
    *   `Tech-浏览器自动化工程师.md`: 浏览器自动化开发。
*   **Tools (工具类)**
    *   `Tools-Github项目管家.md`: Github 项目管理。
    *   `Tools-GitCommit专家.md`: 规范化 Git 提交。
    *   ... (MCP配置、系统可视化等)

## 🚀 如何使用 (Usage)

本仓库只包含整理好的规则文件，**不包含** Trae 的项目配置或原始素材。

### 1. 获取规则
```bash
git clone https://github.com/Cooper-X-Oak/trae-agent-rules-CN.git
```

### 2. 集成到项目
1.  在你的 Trae 项目根目录下，创建 `.trae/rules/` 文件夹。
2.  将 `TRAERULES` 文件夹中的所有 `.md` 文件复制到 `.trae/rules/` 目录下。
3.  **重要**：确保 `RULEOFRULES.md` 和 `Core-中文交互规范.md` 被包含在内，以保证基础体验。

### 3. 验证生效
在 Trae 中打开任意文件或进行对话，AI 将根据当前的上下文（文件类型或你的问题）自动加载相应的规则。

## 🤝 贡献 (Contributing)

欢迎提交 Issue 或 Pull Request 来改进规则库！

1.  Fork 本仓库。
2.  创建特性分支 (`git checkout -b feature/AmazingRule`)。
3.  按照 `RULEOFRULES.md` 的标准编写新规则。
4.  提交更改 (`git commit -m 'feat: Add AmazingRule'`)。
5.  推送到分支 (`git push origin feature/AmazingRule`)。
6.  提交 Pull Request。

## 📄 许可证 (License)

[MIT License](LICENSE)

---
*Created with ❤️ by Cooper-X-Oak using Trae IDE*
