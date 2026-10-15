# Repository instructions

Read the repository README, the root `CLAUDE.md` when present, and applicable project instructions before changing code. Preserve the project's existing architecture, data boundaries, and required checks.


## Efficient AI-assisted development

For the shared workflow, see the private `core-ai-jp/core-knowledge` guide `AI-COMPANY/AI_DEVELOPMENT_OS/WORKFLOWS/TOKEN_EFFICIENT_DEVELOPMENT.md` when available. Keep these repository instructions and all local security, data, and validation contracts in force.

- Scope the task first. Search paths and diffs, then read only the source, tests, and decisions needed to establish the relevant facts. Reuse verified context and avoid rereading unchanged material; do not omit required company decisions or security context.
- Match the model and reasoning effort to the task: use the lightest option that can complete routine searches or documentation reliably, and escalate only when complexity, uncertainty, or risk requires it. Pass only the relevant evidence when handing work off.
- Keep changes narrow. Use compact JSON only when handing work to another agent, with relevant fields such as `repo`, `task`, `state`, `decisions`, `files`, `checks`, and `blockers`. JSON does not itself reduce tokens; omit irrelevant history.
- Do not repeat identical failed calls. Diagnose the result first; at most one materially changed retry for a safe, read-only operation. Before retrying a write, check whether it already succeeded.
- Run this repository's required checks and the checks that cover changed behavior. For documentation-only edits, verify the diff, links, and privacy. Do not run production probes just to validate documentation.
- Jev is optional for batched, low-risk classification or routing only when already available and authenticated, and only when its total call cost is expected to be lower than the work it saves. Use one batch; review low-confidence or consequential items. Do not use it for writing, summaries, extraction, complex reasoning, or calculations. Do not install it, configure credentials, or invoke a paid API automatically.
- Follow the current owner approval boundary in `core-knowledge`: confirm immediately before money-related execution and before a production change to user-visible appearance. Keep other actions within the explicit task and runtime permissions; preserve technical security safeguards and do not send external messages, expose secrets, or overwrite others' work without authorization.
- Report changes, checks, and unresolved items briefly. Token or credit savings remain unmeasured until usage is compared.
