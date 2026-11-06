# Roadmap

QuantNavigator is at the documentation and product design stage. The milestones
below are planned outcomes, with acceptance criteria for a usable implementation.
None of the application milestones is complete. Scope and sequencing may change
as prototypes are tested; no release dates are announced.

## 1. Workspace and project foundation

Build the standalone application shell with multiple personal workspaces and
separate projects. Define what belongs to a project and how its records persist.
The desktop or web delivery model remains open.

Acceptance: a user can create two workspaces, add separate projects, close and
reopen the application, and recover each project's saved records without mixing
them with another project's records.

## 2. First external runtime

Select and implement an initial connection from the planned Codex, Claude Code
and Pi integrations. Define how the application starts work and exposes runtime
status, outputs and failures.

Acceptance: a user can start a bounded task in a project, inspect its execution
status and outputs, and identify an interrupted or failed attempt. Document the
tested runtime version, prerequisites and unsupported operations. Additional
runtime connections are separate deliverables with their own verification.

## 3. Persistent research workflow

Connect research questions to experiment plans, configurations and result
artifacts. Preserve unsuccessful attempts and human decisions alongside completed
work. Make those project records accessible independently of an active runtime
session.

Acceptance: a user can reopen a project after a session ends, trace a reported
result to its saved configuration and artifacts, inspect a failed attempt, and
record why a hypothesis was retained, revised or rejected.

## 4. Quantitative research tools

Introduce tools for data checks, temporal validation and baseline comparisons,
followed by result inspection and reports. Reports should expose provenance,
periods evaluated and limitations alongside metrics and plots.

Acceptance: a documented example can be reproduced from its stated inputs and
configuration. A reviewer can inspect its validation split, compare the candidate
with a baseline, and follow each reported metric or plot to the underlying
result artifact. Example data and demonstration results must be labeled.

## 5. Extension interfaces

Define plugin interfaces around concrete research needs. Introduce research
capabilities gradually as plugins or native components, with documented data
contracts and boundaries.

Acceptance: an example plugin adds a research operation or result view through a
documented interface. Its inputs and outputs are inspectable, and a plugin
failure is reported without losing existing project records. Document the
supported interface version and compatibility limits.

## 6. Native runtime

Evaluate Pi and Mastra as foundations for a native QuantNavigator runtime.
Choose an approach against explicit requirements before committing to a framework.

Acceptance: record the selection criteria and tradeoffs, then demonstrate a
bounded research task using the chosen implementation. The user can inspect
execution, recover the saved project records after interruption, and review the
result before deciding what runs next. Document differences from external
runtime integrations.

## Decisions still open

The application delivery model, first external runtime, plugin interfaces and
native runtime foundation require design and prototype evidence. Runtime feature
parity and transfer of complete internal sessions are outside the current plan.

The roadmap covers the research environment and its tools. It contains no
profitability targets or live order execution milestone.

Return to the [project overview](README.md).
