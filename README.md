# Claude-Skils-by-Wizzo
Custom Skills for Claude AI — reusable workflows for resumes, documents, and everyday tasks.
xWhat's a Skill?

A Skill is a folder containing a SKILL.md file (plus optional scripts, templates, and reference docs) that tells Claude how to approach a particular kind of task. When the description matches what you're asking for, Claude automatically loads the skill and follows its workflow.

Skills in this repo

SkillDescriptionresume-builderCreates personalized, ATS-friendly resumes as Word documents, tailored to a specific job posting.


Add a row here each time you add a new skill.



Installation

Each skill is packaged as a .skill file. To use one:


Download the relevant .skill file from this repo (or build one from its source folder using the skill-creator skill's package_skill.py script).
Upload/install it into your Claude environment (Claude.ai, Claude Code, or Cowork) following Anthropic's skill installation instructions.


Alternatively, clone this repo and point your Claude setup at the individual skill folders directly.

Repository structure

.
├── resume-builder/
│   └── SKILL.md
├── ...
└── README.md

Each skill lives in its own top-level folder named after the skill, containing at minimum a SKILL.md with YAML frontmatter (name, description) and the workflow instructions.

Adding a new skill


Create a new folder at the repo root, named after the skill (lowercase, hyphenated).
Add a SKILL.md with:

name: the skill identifier
description: when Claude should use this skill and what it does
The body: step-by-step instructions for Claude to follow



Add any supporting scripts/, references/, or assets/ the skill needs.
Update the table above with the new skill.
(Optional) Test the skill and package it as a .skill file for easy distribution.


License

This repository is licensed under the MIT License.
