# Draft a post

Triggered by a task that names one piece, or by an idea you have decided is worth writing. Budget 45
minutes. The outcome is one finished draft in `reports/`, its short versions, and a task note a person
can approve from.

## 1. Decide it is worth writing
    hub task show <id>

It is worth a piece when it answers a question a real reader has, the company can say it truthfully
and specifically, and it is not what the last two pieces said. If it fails any of those, say so in one
line on the task and add it to `knowledge/ideas.md`.

## 2. Read before you write
- `knowledge/voice.md`, always, before the first sentence.
- `knowledge/company.md`, for what is true and what must never be claimed.
- The last two pieces in `reports/`.
- Whatever the idea's source actually said, in full. A summary of a summary says nothing.

## 3. Write the piece
`reports/YYYY-MM-DD-<slug>/post.md`:
- Open with the concrete thing: a recognizable situation or the result.
- One point, supported, then stop.
- No number, quote, testimonial, or result you did not read in a dated source. Mark gaps
  `[NEEDS SOURCE: ...]`.
- No guarantee, no unsourced comparison, no promise about an outcome.

Then `notes.md` in the same folder: each claim, its source, and its date. Then the short versions the
channels need, one file each, as cuts of this piece and not new pieces.

## 4. Check it
Run `playbooks/edit-a-draft.md`. If the second read against `knowledge/voice.md` fails twice after
rewriting, stop: keep it as internal work and say so. Do not ask a person to rewrite it for you.

## 5. Hand it over
Commit, then `hub task update <id> --status done --note`: what the piece says in one line, the folder
path, what is still missing, and one line on what you would do once a person approves. When the owner
wants it out, that is `hub approval request` with the exact text and destination. You never publish.

## 6. Keep the plan honest
Move this piece from planned to drafted in `knowledge/plan.md`, and put anything this run taught you
about what to write next in `knowledge/ideas.md`, with where it came from.
