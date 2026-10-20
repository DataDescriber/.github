# Reporting and following up work

Report in the repository responsible for the affected service or feature. Follow
that repository's more specific contribution and incident-response instructions
when present.

## Before filing

Search open and closed issues and relevant pull requests using the symptom,
affected feature, monitoring identifier, and alternative wording. Look in related
repositories when responsibilities cross their boundaries. Read plausible matches;
similar titles alone do not establish duplicates. Add new evidence to existing
work when it covers the same outcome. Incomplete access or search results do not
prove that no related work exists.

## Choose the right report

- **Production incident:** confirmed production disruption or degradation. Describe
  the failure, time and environment, observed impact, and current condition with
  its observation time. Do not delay established incident response to finish a form.
- **Bug or suspected incorrect behavior:** describe the action or conditions,
  actual result, expected result and why it is expected, and reproduction and
  environment information when known. A reported bug is not necessarily reproduced.
  A monitoring error without confirmed impact belongs here as a suspected bug.
- **Improvement or new capability:** describe who needs what, the current limitation,
  and the desired outcome with a concrete example. A suggested solution is a
  proposal, not an accepted requirement.

The body must explain the problem without requiring access to another system.
Include only necessary, sanitized evidence. Keep sensitive details in an
appropriate protected source; do not paste secrets, personal information,
customer data, or raw diagnostic dumps into issues or comments.

## Triage and information placement

Maintainers establish scope, priority, and observable closure criteria during
triage. Mark proposals as proposed until agreed. A reporter does not need to
supply a diagnosis, implementation plan, or finished acceptance criteria.

| Location | What belongs there |
| --- | --- |
| Issue body | Current self-contained problem or need, relevant observations and evidence, known uncertainty, agreed scope, and verifiable closure criteria |
| Issue comments | Investigation findings, reproduction attempts, hypotheses, rejected explanations, decisions, and reasons for scope changes |
| Implementing PR | That PR's changes and rationale, criteria it covers, verification and limitations, and relevant delivery or rollback details |

Update the body as understanding changes while preserving the original
observations and distinguishing corrections from hypotheses. Record the reason
for material changes in a comment. Promote decisions affecting scope or behavior
into the body or an authoritative linked specification.

Do not turn the body into an investigation diary or duplicate changing PR state,
head SHAs, CI results, or implementation test commands. Reproduction steps belong
in the bug report; verification of an implementation belongs in its PR.

## Independent outcomes and partial delivery

Use separately closeable issues when outcomes can usefully be prioritized or
delivered independently. Each part needs a clear scope, acceptance criteria, and
links to its implementation.

Use GitHub's native sub-issues when the parts together satisfy the parent's goal.
Use related independent issues for separate improvements, and blocked-by
relationships only for actual prerequisites. Keep the parent's original problem
and overall goal visible, using native progress rather than copied PR status.

A PR should close only the issue or part it resolves. Use a non-closing reference
for a parent whose required outcomes remain. Deferred work needs an explicit home
and remaining scope; deferred does not mean done. Not every discovery in an
investigation becomes a condition for closing the original report.

Track restored service and permanent correction separately when their outcomes
or priorities warrant it. Close incidents using evidence of the agreed recovery
conditions. Distinguish implementation, verification, merge, and deployment:
a merged PR alone does not establish restored production behavior.

## Reviewing an implementation

Explain the problem and resulting behavior first, then the changes needed to
understand the approach. Identify the issue criteria covered by this PR and any
remaining work elsewhere. State the checks actually performed, their results and
limitations, and what reviewers should inspect. Keep deployment and rollback
details in the PR when relevant.

Follow the target repository's review and signing requirements. Read back
published changes and links before reporting completion.
