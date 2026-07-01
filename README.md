# readme-generator

从现有代码仓库生成实用的工程 README。

## 能做什么

- 分析项目结构、脚本、构建文件、日志和已有文档。
- 生成面向研发同学的 `README.md`。
- 覆盖快速开始、工程结构、构建命令、日志调试、研发流程和 FAQ。
- 对缺失信息使用 `TODO` 标记，不编造项目事实。

## 仓库结构

- `SKILL.md`：唯一的 skill 定义文件，同时适用于 Codex 和 Cursor Agent Skills。

## 添加到 Codex

把仓库克隆到 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/zhonglaoban/readme-generator.git ~/.codex/skills/readme-generator
```

之后在 Codex 中要求生成、更新、改进或重写项目 README 即可触发。

## 添加到 Cursor

Cursor Agent Skills 使用 `.cursor/skills/<skill-name>/SKILL.md` 结构。把本仓库的 `SKILL.md` 复制到目标项目：

```bash
mkdir -p .cursor/skills/readme-generator
cp path/to/readme-generator/SKILL.md .cursor/skills/readme-generator/SKILL.md
```

也可以在 Cursor 中从 GitHub 导入：

1. 打开 Cursor 的 **Customize**。
2. 进入 **Rules**，点击 **Add Rule**。
3. 选择 **Remote Rule (Github)**。
4. 输入 `https://github.com/zhonglaoban/readme-generator`。

安装后，让 Cursor 生成或改进当前项目 README。

---

## English

Generate practical engineering `README.md` files from an existing codebase.

## What It Does

- Inspects project structure, scripts, build files, logs, and existing docs.
- Writes a concrete developer-facing `README.md`.
- Covers quick start, project structure, build commands, logs, debugging, workflow, and FAQ.
- Marks missing information with `TODO` instead of guessing.

## Repository Layout

- `SKILL.md`: the single skill definition file for both Codex and Cursor Agent Skills.

## Add to Codex

Clone this repository into your Codex skills directory:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/zhonglaoban/readme-generator.git ~/.codex/skills/readme-generator
```

Then ask Codex to create, update, improve, or rewrite a repository README.

## Add to Cursor

Cursor Agent Skills use `.cursor/skills/<skill-name>/SKILL.md`. Copy this repository's `SKILL.md` into your target project:

```bash
mkdir -p .cursor/skills/readme-generator
cp path/to/readme-generator/SKILL.md .cursor/skills/readme-generator/SKILL.md
```

You can also import it from GitHub in Cursor:

1. Open **Customize** in Cursor.
2. Go to **Rules** and choose **Add Rule**.
3. Select **Remote Rule (Github)**.
4. Enter `https://github.com/zhonglaoban/readme-generator`.

After installation, ask Cursor to generate or improve the project README.
