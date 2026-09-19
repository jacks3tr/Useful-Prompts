Audit this repository for real, actionable bugs using STATIC CODE INSPECTION ONLY. Investigate and report. DO NOT fix anything.

BOUNDARIES
Do not modify project files, install dependencies, change configuration, commit, or open pull requests. Preserve existing uncommitted work.

DO NOT run test suites, individual tests, builds, scripts, the application, reproduction attempts, browser interactions, or live/API checks. Do not execute project code or contact external systems. Reading existing tests is allowed. Use read-only file inspection and search only.

INVESTIGATION
Read repository instructions and establish intended behavior. Inspect relevant implementations, callers, guards, and downstream effects.

Prioritize security and authorization failures, data loss or corruption, incorrect business logic, broken integrations, concurrency issues, persistence/restart failures, and error-handling defects.

Exclude style preferences, refactoring opportunities, feature requests, and unsupported hypotheticals. Do not manufacture findings to meet a quota.

STOP RULE
This is bug discovery, not exhaustive verification. Make one focused code-review pass per candidate. Once a concrete code path supports the finding, record it and move on. If evidence remains inconclusive, mark it unverified, state what is missing, and move on. Do not repeatedly revisit findings or attempt runtime proof. Deeper verification belongs to Part 2.

REPORT
Order findings by severity. For each bug include:
- Severity and concise title.
- Exact file path and smallest relevant line range.
- Triggering conditions and concrete failing code path.
- Expected versus actual behavior and practical impact.
- Supporting code evidence.

Separate code-supported findings from unverified concerns. Deduplicate findings sharing the same root cause. Clearly state that findings come from static analysis and were not runtime-tested.

Finish with areas inspected and coverage limitations. If no bugs are substantiated, say so without declaring the repository bug-free.

Return the report in chat, without patches or file changes. Stop after reporting.
