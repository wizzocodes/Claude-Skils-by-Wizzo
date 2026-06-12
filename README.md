# 🧩 Claude Skills by Wizzo

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Made for Claude](https://img.shields.io/badge/Made%20for-Claude%20AI-6A5ACD)](https://claude.ai)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#contributing)

> A curated library of custom **[Claude Skills](https://docs.claude.com)** — reusable, drop-in workflows that teach Claude how to handle specific tasks, from building ATS-friendly resumes to automating documents.

---

## ✨ What's a Skill?

A **Skill** is a folder containing a `SKILL.md` file (plus optional scripts, templates, and reference docs) that tells Claude *how* to approach a particular kind of task. When your request matches a skill's description, Claude automatically loads it and follows its workflow — no extra prompting needed.

---

## 📦 Skills in this repo

| Skill | Description |
|-------|-------------|
| 📄 [`resume-builder`](./resume-builder) | Creates personalized, ATS-friendly resumes as Word documents, tailored to a specific job posting. |

> 💡 Add a new row here every time you publish a new skill.

---

## 🚀 Installation

Each skill is packaged as a `.skill` file. To use one:

1. Download the `.skill` file for the skill you want from this repo.
2. Upload/install it into your Claude environment (Claude.ai, Claude Code, or Cowork) following Anthropic's [skill installation instructions](https://docs.claude.com).

Alternatively, clone the whole repo and point your Claude setup at the individual skill folders directly:

```bash
git clone https://github.com/<your-username>/<this-repo>.git
```

---

## 🗂️ Repository structure

```
.
├── resume-builder/
│   └── SKILL.md
├── ...
├── LICENSE
└── README.md
```

Each skill lives in its own top-level folder named after the skill, containing at minimum a `SKILL.md` with YAML frontmatter (`name`, `description`) and step-by-step instructions.

---

## 🛠️ Adding a new skill

1. Create a new folder at the repo root, named after the skill (lowercase, hyphenated).
2. Add a `SKILL.md` with:
   - `name` — the skill identifier
   - `description` — when Claude should use this skill and what it does
   - The body — step-by-step instructions for Claude to follow
3. Add any supporting `scripts/`, `references/`, or `assets/` the skill needs.
4. Update the **Skills in this repo** table above.
5. (Optional) Package the skill as a `.skill` file for easy distribution.

---

## 🤝 Contributing

Contributions, ideas, and new skills are welcome! Feel free to open an issue or submit a pull request.

---

## 📄 License

This repository is licensed under the [MIT License](./LICENSE).
