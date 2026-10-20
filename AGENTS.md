# Agent guidance

## Scope

Maintain public organization defaults: issue forms and their chooser configuration,
shared contribution guidance, and documentation for this repository. These instructions
apply here; they are not automatically inherited by other repositories.

## Reporting principles

- Choose between confirmed production incidents, observed or suspected bugs, and
  improvement requests. A telemetry source does not determine the report type.
- Make the problem understandable in the issue body without opening external evidence.
  Preserve unknowns; do not promote hypotheses or proposals into facts or requirements.
- Issue bodies hold the current problem, agreed scope, and closure criteria.
  Comments record investigation and decisions. Implementing PRs record their own
  changes, covered criteria, verification, and relevant delivery details.
- Split independently prioritizable or deliverable outcomes when useful. Use native
  sub-issues for required parts of the parent's goal and related independent issues
  for separate improvements. Deferred work is not complete.
- Keep human forms usable before triage. Do not require a diagnosis, repeatable
  reproduction, implementation plan, or finished acceptance criteria to file a report.
- Keep these principles aligned with the maintained GitHub issue-management skill;
  do not embed agent workflow instructions in human-facing form submissions.

## Public content and portability

Everything here, including history, is public. Do not copy private repository
history, internal incident details, credentials, customer information, or private
diagnostics into this repository. Use generic examples.

Do not configure global labels, issue types, assignees, projects, or contact
destinations without verifying they are valid for the intended repositories.
Local issue-template configuration replaces the whole shared set; it does not
extend it. Prefer central defaults and deliberate exceptions over distributed copies.

## Change and verification

Inspect the working tree, current default branch, open work, and GitHub rules.
Preserve unrelated changes. Use `feature/` branches, signed Conventional Commits,
and focused PRs for changes after initialization. Do not merge, enqueue, enable
auto-merge, bypass rules, add AI attribution, or change global Git configuration.

For form edits, parse YAML, check GitHub's form schema, unique form names and field
IDs, required-field choices, and linked guidance. Exercise realistic incident,
suspected-bug, and improvement reports without submitting test issues. Check the
GitHub chooser and forms after publication; distinguish local validation from
hosted acceptance and inheritance.

Keep drafting files and evidence in persistent local storage outside the public
tracked content. Confirm the exact staged diff before pushing. Read back remote
content and visibility after publication.
