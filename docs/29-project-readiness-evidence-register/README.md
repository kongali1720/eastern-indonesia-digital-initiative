# Project Readiness & Evidence Register

## Purpose

Track project requirements, accountable owners, supporting evidence,
verification, approvals, due dates, and follow-up actions in one register.

This register is a planning and governance control. It does not independently
authenticate documents, certify funding, establish legal compliance, or prove
that a project milestone has been completed.

## Status definitions

- `Proposed`: requirement identified; work or evidence not yet established.
- `In Progress`: an owner is working on the requirement.
- `Evidence Submitted`: a supporting reference has been recorded but not yet verified.
- `Verified`: evidence has been reviewed by an identified reviewer and a verification date is recorded.
- `Approved`: the applicable decision has been approved and an approval reference is recorded.
- `Blocked`: progress is blocked; record the reason and next action in the notes or next-action field.

Use only these status values. Do not mark an item Verified or Approved merely
because a reference field is populated.

## Required control fields

- `readiness_id`: unique requirement identifier.
- `workstream`: project workstream or discipline.
- `requirement`: clear, testable readiness requirement.
- `status`: current status from the definitions above.
- `owner`: person accountable for the next action.
- `evidence_reference`: path, document ID, or controlled reference to supporting evidence.
- `evidence_date`: date associated with the evidence, where applicable.
- `verified_by` and `verified_date`: reviewer and review date.
- `approval_reference`: decision or approval reference when applicable.
- `next_action` and `due_date`: follow-up and target date.
- `notes`: limitations, dependencies, and unresolved issues.

## Dashboard interpretation

The dashboard displays the number of loaded requirements. Its Verified count
includes rows marked Verified or Approved only when evidence reference,
reviewer, and verification date are all present. Its Approved count includes
Approved rows only when an approval reference is present. Blocked counts are
based on the Blocked status.

These are register completeness checks, not independent authentication of the
underlying evidence. Keep source documents in an access-controlled location;
do not place confidential personal, financial, or security information in a
public repository.

## Reporting discipline

- Use `Unknown` or leave fields blank when information has not been confirmed.
- Do not invent owners, dates, evidence, approvals, or readiness claims.
- Record the source and date of material updates.
- Review overdue actions and blocked items at each project governance meeting.
