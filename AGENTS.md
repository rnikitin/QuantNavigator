# Contributor guidance

This repository is at the documentation and product design stage. Application
code and runtime integrations have not been released. Read README.md and
ROADMAP.md before changing the product description.

- Use English for public documentation, interface text and identifiers.
- Distinguish planned capabilities from implemented and verified behavior.
- Keep secrets, private documents, personal data and internal paths out of the
  repository. Do not commit raw market data, model weights or run artifacts.
- Keep documentation links valid and check changes for whitespace errors with
  `git diff --check`.
- Document build, installation and test commands only after they exist and have
  been verified. Documentation checks do not verify application behavior.
- Preserve LICENSE and source attribution when adapting external material.

## Required coding skill

Before implementation, debugging, refactoring, test edits or code review, load
and apply [karpathy-guidelines](.agents/skills/karpathy-guidelines/SKILL.md).
Read the full file when first needed in a session, and again after context loss
or a material change to the skill source. If host skill discovery does not list
it, read the local path directly. Naming the skill does not count as loading it.
Existing scope, authorization and verification policies continue to apply.
