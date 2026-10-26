<p align="center">
  <img src="assets/logo-pivotal.png" alt="Pivotal Logo" width="100">
</p>

<h1 align="left">Pivotal</h1>

Pivotal is a portable, self-contained AI coding instruction system distributed through a single `AGENTS.md` file. It is designed to help compatible AI coding agents understand user intent, work efficiently, avoid unnecessary complexity, reuse existing solutions, and verify results before reporting completion.

By providing structured operational guardrails, Pivotal is designed to improve an agent's understanding of project context, reduce redundant exploration and overengineering, encourage the reuse of established code, and promote proportional verification before declaring tasks complete—all without requiring software installations, package dependencies, or runtime configuration.

## ✨ Key Features

- **Intent & Context First**: Guides agents to determine actual user objectives, evaluate available context, and distinguish explicit requirements from assumptions before acting.
- **Solution-Priority Ladder**: Directs agents to evaluate solutions in priority order (no change, existing code, standard library, native platform features, installed dependencies, and minimal custom code) before introducing new code.
- **Smallest Complete Solution**: Encourages the simplest maintainable approach that fully satisfies requirements without introducing unrequested abstractions or fragile implementations.
- **Targeted Exploration & Efficiency**: Designed to curb unnecessary token usage, aimless repository scans, redundant tool calls, and repeated actions without root-cause assessment.
- **Blast Radius Control**: Preserves working architecture, untouched files, and formatting conventions while avoiding unsolicited refactoring or extraneous dependencies.
- **Quality & Safety Considerations**: Reminds agents to uphold security boundaries, input validation, data integrity, accessibility standards, and essential regression tests.
- **Proportional Verification**: Promotes matching verification effort to task risk, requiring concrete execution evidence and diff reviews before declaring completion.
- **Portable & Zero-Dependency**: Delivers full operational guidance through a single standalone `AGENTS.md` file with no tools to install or configure.

## 🚀 How to Use Pivotal

Using Pivotal is straightforward and requires no build tools, packages, or runtime setup.

### Step 1 — Download the Instructions

Download [`AGENTS.md`](https://github.com/evanhendramulyadi/pivotal/blob/main/AGENTS.md) from this repository, or grab the [raw file directly](https://raw.githubusercontent.com/evanhendramulyadi/pivotal/main/AGENTS.md).

### Step 2 — Place `AGENTS.md` in Your Project

Copy `AGENTS.md` into the root directory of the project you want to work on:

```text
your-project/
├── AGENTS.md
├── index.html
├── package.json
└── ...
```

- Place `AGENTS.md` in the project root alongside files like `package.json` or `.git`.
- Copy the file into your existing project; do not replace your project folder.
- If your target project already has an `AGENTS.md`, review and merge the instructions rather than blindly overwriting existing rules.

### Step 3 — Open the Project in an AI Coding Agent

Open your project in a compatible AI coding agent or IDE that supports `AGENTS.md`.

> [!NOTE]
> AI coding tools handle instruction files differently. Behavior depends on the specific tool, its version, and its instruction-loading mechanism. If your tool expects an alternative instruction file convention (such as `.cursorrules` or `CLAUDE.md`), you can copy or reference the contents of `AGENTS.md` within that file.

### Step 4 — Start Coding

Give your coding agent tasks as you normally would. For example:

> Build a responsive login page using the existing project structure. Reuse available components and dependencies, avoid unnecessary complexity, and verify the implementation.

Pivotal provides project-level instructions for the agent to follow; it guides the agent's working discipline but does not replace the AI coding agent itself.

## ⚙️ How Pivotal Works

Pivotal organizes agent behavior around an adaptive, six-stage operational rhythm:

`Understand → Inspect → Prioritize → Execute → Verify → Report`

1. **Understand**: Clarify user intent, requirements, constraints, and success criteria before taking action.
2. **Inspect**: Examine only the files, callers, and dependencies directly involved in the task.
3. **Prioritize**: Evaluate solutions using the Solution-Priority Ladder, favoring existing code and platform features before writing new code.
4. **Execute**: Implement the simplest maintainable change that satisfies the requirements while preserving existing architecture.
5. **Verify**: Validate changes proportionally using relevant tests, linters, builds, and diff reviews.
6. **Report**: Summarize what was changed, provide verification evidence, and note any remaining caveats or limitations.

## 🧩 Compatibility and Requirements

- **Distribution Format**: Pivotal is distributed entirely as a standard Markdown instruction file (`AGENTS.md`).
- **Zero Runtime Dependencies**: Pivotal requires no installation commands, runtime environments, build processes, package managers, or external dependencies.
- **Agent Integration**: The instructions are intended for AI coding agents and development environments that support or can be configured to read `AGENTS.md`. Different tools may load and handle instruction files differently.
- **Variable Outcomes**: Actual results depend on the specific AI agent, its model capabilities, available context, and how closely it follows workspace instructions. Pivotal does not claim universal compatibility or guaranteed compliance across all tools.

## 📁 Repository Structure

```text
Pivotal/
├── AGENTS.md
├── README.md
├── LICENSE
└── assets/
    └── logo-pivotal.png
```

- **`AGENTS.md`**: The actual product. This is the only file you need to copy into a compatible coding project.
- **`README.md`**, **`LICENSE`**, and **`assets/`**: Repository documentation, licensing information, and assets; they are not required at runtime in your project.

## 📄 Copyright & Ownership

© 2026–Present Evan Hendra Mulyadi.

Pivotal is an open-source project created by **Evan Hendra Mulyadi**. It is made available for public use, study, modification, and redistribution under its applicable open-source license.

The project encourages the community to use, adapt, improve, and build upon Pivotal in accordance with the terms of its license.

The project encourages the community to use, adapt, improve, and build upon Pivotal in accordance with the terms of its license.