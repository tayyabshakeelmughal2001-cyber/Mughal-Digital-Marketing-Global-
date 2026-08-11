# SECURITY_TRIAGE.md

Purpose

This file documents a concise, repeatable triage process for CodeQL (Code Scanning) alerts so security and quality issues are reviewed and actioned promptly.

Quick triage checklist

1. Acknowledge new alerts within 48 hours.
2. Classify each alert: Critical / High / Medium / Low / False Positive.
3. For Critical/High alerts:
   - Create an issue titled: "[CodeQL] <short description>"
   - Assign the issue to a maintainer and set a milestone or target sprint.
   - Link any fix PRs to the issue and to the alert.
   - Track progress and close the alert when the fix is merged.
4. For Medium alerts:
   - Investigate and create an issue if the finding requires work.
   - Schedule the fix in the next sprint or backlog with priority.
5. For Low alerts:
   - Log the finding in the backlog; re-evaluate on a quarterly security review.
6. For False Positives:
   - Add a short comment on the alert explaining why it is a false positive and mark it "No fix planned" or dismiss according to policy.

Severity and SLAs

- Critical / High — create issue and aim to fix within 7 days.
- Medium — investigate and schedule within the next 1–2 sprints.
- Low — monitor and fix as part of routine maintenance.

Triage owner

- Primary: @tayyabshakeelmughal2001-cyber
- If unavailable, assign to another maintainer and note in the alert comments.

How to document decisions

- Use GitHub issues for tracking fixes. Link PRs to the issue and include the CodeQL alert url in the PR description.
- When dismissing or marking an alert as false positive, leave a short rationale in the alert comments so future reviewers understand the decision.

Useful commands / examples

- To link a PR to an alert: include the alert URL in the PR description and reference the issue number.
- Example issue title: "[CodeQL] Unsafe use of eval in utils/parser.js"

Contact

If you are unsure how to triage a finding, open a discussion or assign the alert to @tayyabshakeelmughal2001-cyber.
