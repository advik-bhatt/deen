# deen — agent rules

Global rules live in `advik-bhatt/knowledge-base` → CLAUDE.md (branch
discipline: all work commits directly to main, no worktrees, no feature
branches; commit author Advik Bhatt <advik.bhatt@gmail.com>; no model IDs
in commit messages).

## Public record: verbatim, no filter (founder, Jul 26 2026)

deen is public and stays public; open-sourcing the work is the point.
The profanity filter on founder quotes is rescinded — quotes land
verbatim, cursing included. Naming his diagnoses (ADHD, OCD, anxiety
disorder) is fine on any surface here; he is open about them.

The one boundary that stands: **no private experiential detail.**
Specific episodes, session content, prompt history, and anything else
from the private log never lands in deen — that material lives in the
private knowledge-base only. Only the public research is pushed here.
When in doubt: publish the research, keep the experience private.

## Merge desk (multi-thread pushes)

Parallel Claude threads share `main`. Never raw `git push`; push via
`sh .claude/merge-desk/sync-push.sh` (rebases, retries races, files a
conflict card on real collisions). On exit 42 follow the merge-desk skill
(`.claude/skills/merge-desk/`): resolve intent-first, then post the card
as a GitHub issue titled `[merge-desk] deen: <plain summary>` so Advik can
approve, change, or revert. At session start, apply approved
`[merge-desk]` cards first and announce your goal on the
`[merge-desk] Thread board` issue.
