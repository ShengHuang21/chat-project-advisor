# Evidence and Handoff

Match the strength of a statement to the evidence available.

- **Confirmed:** directly supported by current, relevant evidence.
- **Inference:** a reasoned conclusion that should name its basis and limit.
- **Unknown or pending:** not established; say what minimal evidence or decision would resolve it.

When reviewing a handoff or reuse decision, capture only the fields needed to avoid a misleading claim: the intended outcome, relevant change/scope, evidence observed, checks run or not run, environment or configuration boundary when relevant, remaining limitation, and the owner or authority needed for a next external action.

For a detailed Todo, also record the single formal owner, the advisory recommendation, and whether Codex accepted, partially accepted, or rejected it with a short evidence-based reason. Acceptance is a decision, not a passed check. Keep a common background's version, required core, task delta, and known gap distinct from evidence of current behavior.

Old evidence may still be useful if the relevant implementation, dependencies, configuration, environment, and acceptance scope have not materially changed. Re-evaluate the affected boundary when they have. A matching revision identifier can help locate evidence but is not, by itself, the test for relevance; conversely, mandatory exact-revision checks cannot be skipped merely because other evidence appears reusable.

Do not convert local observations into broader claims: a successful local check does not alone prove release, deployment, customer effect, or acceptance. If the source cannot be accessed, report the limited conclusion and request only the approved, decision-changing excerpt or result.

## Initial coverage and material availability

For the first consultation on a binding, ask the bound Codex to assemble the task-relevant material proactively from approved existing sources. Assess these six coverage areas together, so obvious dependencies are not discovered one prompt at a time:

| Coverage area | Relevant material |
| --- | --- |
| Task and boundary | Goal, observable Done, current stage, requested output, scope, owner, and applicable authority |
| Understanding and background | Approved common core/version, repository and task background, ownership/data-flow/architecture understanding, and relevant diagrams with companion Markdown |
| Plan and reasoning | The single formal Todo and revision, local investigation/analysis, decisions and unresolved hypotheses |
| Observed collaboration state | GitHub repository/PR identity, refs, review findings, CI runs/results and observation times; distinguish unavailable state from no findings or passing checks |
| Fixed source and execution chain | Relevant diff and candidate files, interfaces/tests/safe configuration, and applicable workflow, Terraform, or deployment chain |
| Work and verification | Actual work records, human observations/approvals within their scope, tests, failures, omitted checks, limitations, and remaining gaps |

These are coverage areas, not six mandatory files or a request for all material. Reuse overlapping sources once; mark genuinely irrelevant areas not applicable with a short reason. A small review needs only material relevant to its decision. Completeness means accounting for relevant coverage, including gaps, not claiming every area is proven.

Include a compact material availability menu with source/version and decision impact. Reference the existing material manifest, fixed ref or frozen overlay, and file path/range instead of creating a competing inventory. Bind test/CI evidence to its result link or record, run/attempt/job where applicable, tested version, and environment:

- **Supplied and readable here:** identify what the advisor can actually inspect, including received parts and redactions. A named attachment or local link alone is not readable evidence.
- **Available via local Codex:** name the approved source or bounded item Codex can collect and send, without claiming the advisor has already read it. Same-version availability requires a retrievable fixed Git object or frozen body; an old path or hash alone leaves recoverability unconfirmed.
- **Inaccessible, not collected, or excluded:** distinguish these states and say which conclusion is limited. Record why an item is excluded, redacted, or not applicable; never silently interpret absence as success.

If the approved common core is relevant, read it on the first binding together with the task delta and necessary repository/task background. Diagram companion Markdown should preserve components, relationships, ownership and deployment boundaries, source/version, and gaps. A path to an image does not transmit its pixels; base judgments on supplied text unless the image itself was actually received and inspected. Do not claim visual verification from a description.

Keep Skills, tools, and data sources distinct in the menu. A local Skill has a verified name, purpose, availability, and access route; naming it does not make it remotely callable. A document repository or shared folder is a source, while a service connector is a tool, not a Skill. Do not invent names or imply installation or access from a reference alone.

The cloud advisor cannot directly call local Skills, inspect private repositories, open local paths, or read a ZIP from its name. It requests a specific same-version item from the bound Codex and explains the affected decision. The existing authorized native local send/read loop handles collection and exchange; this skill adds neither transport nor send authority. If that loop or source is unavailable, report the gap and a bounded partial judgment rather than inventing access or making the user repeat a locally available packet by default.

## Binding, deltas, and recovery

In a task-bound local advice loop, separately record that a message was sent, a response was read, and advice was integrated. Do not treat any one state as the others, and use the original task record for concise de-duplication and resumption notes. A response is advisory, not an authorization or a replacement for the formal Todo owner.

For a bound consultation, have the advisor reproduce the task, request, material, and binding identities in its reply. Preserve those returned identities unchanged in the task record. If an identity is missing or conflicts, do not assume the intended context or automatically integrate the advice; resolve the mismatch against the current task record. This supports task-local reasoning, not confidentiality isolation in a shared Chat.

For the same binding, send relevant task/source/background changes and missing sections as deltas, referencing the frozen material they update. Include current read scope and decision-changing gaps in the substantive reply; do not add a separate routine memory-check turn. Reused evidence must remain applicable. A new binding needs a complete task-relevant initial packet, including its required common core, even if another Chat received it earlier.

Do not promise to detect the exact timing or contents of another Chat's context compaction. Returned identities, a receipt, or an assertion of remembering do not prove that source bodies are currently available. If needed bodies are unavailable or the reply shows a material context gap, recover the required original content from the same frozen version and record what was reread. Do not silently substitute current main or a newer head. If that frozen source cannot be recovered, keep the affected conclusion pending or explicitly limited; do not restart all investigation merely because transport recovery is needed.

## Versioned Source Material

Build a material package from the task's explicitly relevant files, entry points, and interfaces. Do not default to an entire repository, its history, or every branch. For each relevant repository, record its identity and role and acquisition time. Keep these version boundaries separate, even if some resolve to the same commit:

- current **main**, current **PR base** (branch and observed SHA), **merge-base** used for comparison, and candidate **head**;
- approved **local overlay** on that head, including dirty additions, modifications, renames, and deletions with content identities;
- **other relevant refs**, each with a stated reason for inclusion;
- **actual CI checkout**, such as head, a synthetic merge commit, or another ref, bound to the observed run;
- **runtime/deployed revision or image**, environment, observation time, and evidence, or explicitly unknown/not applicable.

When no PR exists, state the intended base and mark PR-only fields not applicable; do not fabricate refs. Record unknown values as unknown. Freeze the material being assessed and record the actual diff comparison endpoints; neither main nor a PR's current base automatically equals its merge-base. A newer main, local overlay, or CI checkout is not silently the reviewed head, and a source revision does not establish the deployed runtime.

The first package normally contains the complete relevant diff, complete candidate versions of affected files, and necessary callers, interfaces, tests, and safe configuration. Supply base or main originals only when the judgment needs them; do not replace an actual PR base with main. Send duplicated content once. The advisor may request a complete same-version file or range when it changes the conclusion.

For a decision-critical behavioral claim, verify that the received body covers the complete relevant function and necessary callers/callees, return/persistence path and side-effect boundary. Text or hash equality proves only the compared content, not semantic sufficiency or whole-repository coverage. Do not infer execution from a function name, signature or validation-only prefix. Distinguish record creation, capability discovery, work claiming, execution start and observed completion; discovery may launch a process without running the user's task. If the body ends before the decisive behavior, give a bounded partial judgment and request the specific same-version continuation or relationship. Correct both overclaims and overcorrections (for example, "does not launch the task" does not mean "has no process side effects"). State actual review coverage, including public source actually read, and keep unproved implementation assumptions conditional. This applies to plan reviews too; do not require unrelated files or a whole-repository audit.

List delivered, omitted, truncated, redacted, and not-applicable items. Give each batch its file list and part/total position. Record source hashes separately from the identity of the content actually sent; a hash helps identify a source but does not let Chat verify bytes it did not receive. Track `sent`, confirmed receipt, and actual review scope separately. Until required material arrives, the advisor may give only a partial opinion; use the recovery rules above when required content is no longer available.

For a deployment-relevant task, include the applicable chain only: source → workflow, reusable workflow, or script → image → Terraform root or module → execution repository/ref → environment. Identify the technical executor and human approver, and record dated runtime evidence or `unknown`. Static configuration does not prove deployment. Do not force this chain on unrelated small tasks.

Keep company material within the authorized target Chat scope. Do not send real `.env` values, credentials, customer data, `.git` contents, caches, artifacts, state files, plans, or unchecked variable files. Do not silently omit security-relevant configuration; when redaction changes meaning, label the resulting advice conditional. Native send is text-only: send versioned batches as text and do not promise ZIP attachments, local-file access, or unattended operation.
