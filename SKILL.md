---
name: readme-generator
description: Use this skill when the user asks to create, generate, update, improve, or rewrite a README for a software engineering repository. It inspects the codebase and existing docs, then produces a concrete Markdown README covering overview, quick start, structure, build, logs, workflow, and FAQ.
---
# README Generator

You are a senior software engineer creating a developer-facing `README.md` from the current repository.

## Workflow

1. Inspect the repository before writing:
   - file tree and major directories
   - existing docs
   - package/build files
   - scripts and CI config
   - logging or troubleshooting conventions
2. Prefer concrete facts from the codebase over generic prose.
3. Write or update the root `README.md`. If a root `README` without extension exists, migrate it to `README.md`.
4. Use compact Markdown with no extra blank lines. Keep necessary newlines inside code blocks.
5. Mark missing information with `TODO`.
6. Include runnable commands whenever possible.

## Required Sections

Use these sections, adapting details to the project type:

- Project Overview
- Quick Start
- Project Structure
- Build
- Logs & Debugging
- Development Workflow
- FAQ

## Section Guidance

Project Overview:
- what the project does
- core capabilities
- technology stack

Quick Start:
- required IDE/runtime/tool versions
- dependency installation commands
- local run/debug commands
- how to verify success

Project Structure:
- important directories and module responsibilities
- key code entrypoints
- where to add new features
- where shared utilities live
- where core logic lives

Build:
- debug build
- release build
- common build commands
- variants, flavors, or schemes when present
- common build failures and fixes

Logs & Debugging:
- how to view logs
- common filters
- debugging tips
- crash log locations
- example commands such as `adb logcat` or `tail -f logs/app.log`

Development Workflow:
- branch conventions
- commit conventions
- code review process
- release process, if discoverable

FAQ:
- environment issues
- build failures
- dependency issues
- startup failures
- login or network problems
- cache problems
