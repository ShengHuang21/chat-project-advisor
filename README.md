# Chat Project Advisor 0.6.1

Source candidate for an ordinary-Chat advisor that helps assess a task plan, bounded versioned source material, verification approach, collaboration design, or handoff. It emphasizes clear goal/Done conditions, warranted counterexamples, minimum sufficient evidence, and authority boundaries.

## Use draft

Ask for a judgment in natural language, for example: “Is this plan sufficient for Done?” or “Can this verification evidence be reused after this change?” Include the intended outcome and any evidence or constraints that materially affect the answer.

For an already bound task advisor, the practical request is: “请让已绑定顾问审查当前Todo”. If the approved background source or the required local send/read capability is unavailable, report that gap rather than claiming this loop is automatically available.

For a code or deployment review, the task owner supplies only the approved, versioned material package for the task and records its scope, missing or redacted items, and response marker. The user need not restate the whole background; the advisor asks for a bounded original file or range only when it changes the judgment.

The single advisor entry follows the task's goal, current stage, and requested output. Bug, feature, and CI work commonly moves from investigation through an evidence-based plan to one formal Todo. Missing evidence calls for bounded investigation; an adequate Todo stays in use, and a CI failure reopens affected steps. A pure PR review ends with findings unless repair scope is authorized.

The advisor accepts sound small plans directly and distinguishes confirmed facts, inference, and unknowns. A Todo review checks ownership, role and model/effort fit, dependencies and parallelism, estimates, test claims, and evidence reuse by default. Codex independently accepts, partially accepts, or rejects the advice; agreement is not proof or a required consensus gate.

The initial task-relevant packet covers task/Done/authority, background and diagram understanding, Todo/local analysis, observed PR/review/CI state, fixed-version source and applicable execution chain, and work/human/test evidence including failures and gaps. These are six coverage areas, not mandatory files. A material menu distinguishes readable supplied content, approved material available via local Codex, and inaccessible/not-collected/excluded items with their decision impact.

The advisor reads the approved common core and relevant background on the first binding, then uses relevant deltas on that binding. A new binding needs its initial packet again. It states actual read scope and gaps in the substantive reply, without routine memory-check turns or promises to detect another Chat's compaction. Needed content is recovered from the same frozen version. Diagram companion Markdown carries the relevant understanding; a local image path is not transmitted pixels. Background remains reference material and is not copied into this package.

The cloud advisor cannot directly invoke local Skills or read a private repository, local path, or ZIP merely because it is named. It requests bounded material from the bound Codex, whose existing authorized native loop handles exchange. The advisor does not dispatch work, change configuration, or push messages proactively. Where an existing task has a bound conversation and local send/read capability, Codex may actively read a reply to close that recorded loop; this neither expands authority nor promises a background service.

## Private account-save path

This package follows the supported private account-save format. For a first save, after the intended account or workspace is confirmed and saving is authorized, save the ZIP through the plugin creation flow. It creates a private plugin in the active workspace, or in the personal account when no workspace is active. For an existing plugin, use its verified identity and current release in a guarded update, then read back the result; preserve the intended audience and `defaultPrompt`.

After a successful save, select **Plugins → Created by you → Chat 项目顾问** in a new ordinary Chat, then ask for a plan or evidence judgment. These are intended steps only; this source and README do not prove the target Chat's save, installation, selection, or validation state.

## Provenance and limitations

This candidate distills neutral decision and delivery principles from the repository's personal planning, reporting, and delivery-review guidance. It does not import their local procedures or make them ordinary-Chat dependencies. It is not an executor, model selector, authority grant, company knowledge package, or proof that a check, release, deployment, or acceptance occurred.

The package excludes `evals/cases.md` and all expected answers. Version `0.6.1` identifies this source candidate only; it is not evidence of the version actually loaded by Chat. Use the external release or validation receipt for the target Chat's actual state rather than changing this README for every release.

Patch 0.6.1 checks semantic coverage separately from source equality: a decision-critical behavioral premise needs the complete relevant function and necessary relationships, or an explicit conditional conclusion. It does not add transport, repository-wide review, or an execution backend.

## Public source distribution

This public repository contains the 0.6.1 source snapshot, including development-only evaluation cases. Publishing source here does not change an existing Chat plugin's audience, install it, or establish that a conversation loaded this version. Exclude `evals/` and its expected answers from runtime packages and evaluated conversations.

The optional local companion is [prepare-advisor-materials](https://github.com/ShengHuang21/prepare-advisor-materials). It prepares approved evidence through local Codex tools; it does not add direct Chat-to-computer access or a transport service.
