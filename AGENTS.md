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

## Karpathy-inspired coding principles

Adapted from the community [Karpathy guidelines](https://github.com/multica-ai/andrej-karpathy-skills/blob/main/skills/karpathy-guidelines/SKILL.md),
inspired by Andrej Karpathy's observations about coding agents.

- Think before coding. Surface material assumptions and tradeoffs before choosing
  an approach. Ask for clarification when ambiguity blocks safe progress; use
  judgment for routine decisions within the authorized scope.
- Simplicity first. Choose the smallest sufficient solution. Add abstractions,
  configuration and features only when the current task needs them. Do not build
  speculative extensions or handle hypothetical requirements.
- Surgical changes. Keep each diff focused on the task. Preserve unrelated work
  and follow the surrounding style. Remove unused imports, helpers and other
  leftovers introduced by your changes; leave unrelated cleanup for a separate
  task.
- Goal-driven execution. Define observable success criteria and use a short plan
  when the work warrants one. Verify in proportion to the change and its risks.
  Mark skipped checks `NOT-RUN` with the missing prerequisite. Continue correcting
  defects until the result is verified within the authorized scope. These
  principles grant no new experiment, paid-call or external-action authorization.
