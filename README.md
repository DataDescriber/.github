# DataDescriber GitHub defaults

Shared issue forms and contribution guidance for DataDescriber repositories.

## Report an issue

Open an issue in the repository responsible for the affected service or feature.
Choose the form that matches what is known:

| Form | Use it for |
| --- | --- |
| Production incident | Confirmed production disruption or degradation |
| Bug or suspected incorrect behavior | Observed or suspected incorrect behavior, including monitoring signals without established impact |
| Improvement or new capability | A need or desired outcome beyond current behavior |

Reports should be understandable directly in GitHub. Supporting links provide
detail; they do not replace the problem description. Diagnosis, reproducibility,
and a finished implementation plan are not prerequisites for reporting.
Blank issues remain available for work that does not fit these forms.

See [CONTRIBUTING.md](CONTRIBUTING.md) for triage, investigation, independently
deliverable work, and the distinction between issue bodies, comments, and PRs.

## How inheritance works

This public repository supplies defaults to DataDescriber repositories, including
private repositories, when they do not define their own corresponding files.
Reports remain in the repository where they are submitted, with that repository's
access controls. Inheriting a form does not publish a private repository or issue.

Forms and their chooser configuration live in `.github/ISSUE_TEMPLATE/` on
`main`. If a repository defines valid local issue templates or local template
configuration, GitHub replaces the entire inherited issue-template set for that
repository; it does not combine local and shared forms.

Prefer these defaults. Add a local override only when a repository has a concrete
reporting need that the shared fields cannot accommodate. An override must provide
all forms that repository needs. Do not install copies in every repository.

A local `CONTRIBUTING.md` takes precedence over shared contribution guidance.
`AGENTS.md` in this repository governs work here; GitHub does not distribute it
as inherited agent instructions.

Authoritative references:

- [Default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [Issue forms](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms)

## Maintain the defaults

Use focused pull requests and signed commits. Validate YAML and preview the
forms in GitHub before claiming that they are usable. Keep reports lightweight:
require the observable problem or need, allow uncertainty, and leave implementation
details to the responsible engineering work.

These forms do not assume particular labels, assignees, projects, or issue types
exist in every destination repository. They also do not determine priority or
replace an established incident-response process.

This repository and its history are public. Keep its contents generic and
suitable for public disclosure. Private organization administration is maintained
separately.
