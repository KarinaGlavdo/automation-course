# Automation Course - Cypress Testing Project

This repository contains a Cypress-based test automation framework designed for end-to-end testing of web applications. The project is configured to work seamlessly with **JetBrains Aqua** IDE.

---

## 📆 Project Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- [Git](https://git-scm.com/)
- [JetBrains Aqua](https://www.jetbrains.com/aqua/) (or any JetBrains IDE)

### Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/KarinaGlavdo/automation-course.git
cd automation-course
npm install
```

---

## 💪 Running Cypress Tests

### Run in Debug (headed) Mode

```bash
npx cypress open
```
Launches the Cypress Test Runner UI for interactive test execution and debugging.

### Run in Headless Mode

```bash
npx cypress run
```
Executes tests in the terminal without opening the UI—ideal for CI/CD pipelines.

---

## 🚀 Git Workflow Strategy

To ensure smooth collaboration, maintainable code, and a clean Git history, the following Git strategy is used:

### Branching Model

- `main`: Stable, production-ready code
- `dev`: Integration branch for ongoing development
- `feature/*`: New features or enhancements
- `bugfix/*`: Fixes for non-critical bugs
- `hotfix/*`: Emergency fixes that go directly to `main`

### Naming Convention Examples

- `feature/login-tests`
- `bugfix/123-fix-timeout`
- `hotfix/fix-broken-login`

### Rules

- Never commit directly to `main` or `dev`
- Open a **pull request (PR)** to merge changes
- PRs must be reviewed and approved
- Use **squash and merge** for clean commit history
- Keep branches up to date via **rebase**, not merge

For more details, see: [Git Strategy Documentation](./docs/git-strategy.md)

---

## ⌨️ Hotkeys for JetBrains Aqua

Boost productivity with these essential JetBrains Aqua hotkeys:

### Navigation

| Action                        | Windows/Linux            | macOS                 |
|-----------------------------|--------------------------|-----------------------|
| Search Everywhere            | `Double Shift`           | `Double Shift`        |
| Find File by Name            | `Ctrl + Shift + N`       | `Cmd + Shift + O`     |
| Find Class                   | `Ctrl + N`               | `Cmd + O`             |
| Find Symbol                  | `Ctrl + Alt + Shift + N` | `Cmd + Alt + O`       |
| Go to Line                   | `Ctrl + G`               | `Cmd + L`             |
| Recent Files                 | `Ctrl + E`               | `Cmd + E`             |
| Last Edit Location           | `Ctrl + Shift + Backspace`| `Cmd + Shift + Delete`|

### File Management

| Action               | Windows/Linux      | macOS           |
|----------------------|--------------------|------------------|
| Project View         | `Alt + 1`          | `Cmd + 1`        |
| Next/Prev Tab        | `Alt + ← / →`      | `Ctrl + ← / →`   |
| Close Tab            | `Ctrl + F4`        | `Cmd + W`        |
| Reopen Closed Tab    | `Ctrl + Shift + T` | `Cmd + Shift + T`|

### Editing & Tools

| Action                   | Windows/Linux      | macOS              |
|--------------------------|--------------------|--------------------|
| Auto-Complete            | `Ctrl + Space`     | `Ctrl + Space`     |
| Quick Documentation      | `Ctrl + Q`         | `F1` or `Ctrl + J` |
| Reformat Code            | `Ctrl + Alt + L`   | `Cmd + Alt + L`    |
| Comment/Uncomment Line   | `Ctrl + /`         | `Cmd + /`          |
| Duplicate Line           | `Ctrl + D`         | `Cmd + D`          |
| Delete Line              | `Ctrl + Y`         | `Cmd + Backspace`  |

### Testing

| Action         | Windows/Linux        | macOS            |
|----------------|----------------------|------------------|
| Run Test       | `Ctrl + Shift + F10` | `Ctrl + Shift + R`|
| Rerun Last Test| `Shift + F10`        | `Ctrl + R`        |

See the full list: [Hotkeys Documentation](./docs/hotkeys.md)

---

## 📁 Project Structure

```
automation-course/
├── .idea/                # JetBrains config (usually .gitignored)
├── cypress/
│   ├── downloads/        # For downloaded files during tests
│   ├── e2e/
│   │   ├── 1-getting-started/
│   │   └── 2-advanced-examples/
│   ├── fixtures/
│   │   └── example.json
│   └── support/
│       ├── commands.js
│       └── e2e.js
├── docs/
│   ├── git-strategy.md
│   └── hotkeys.md
├── node_modules/
├── .gitignore
├── automation-course.iml  # JetBrains module file
├── cypress.config.js
├── package.json
├── package-lock.json
└── README.md

```

---

## 🛠️ Customization

- Update configuration in `cypress.config.js`
- Add global commands in `cypress/support/commands.js`

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

Happy testing! 🚀

