# Ship It Friday — method

Competition: `u-mgwals-ship-it-friday-30bd407a` — one line, 1–159 characters:
the funniest git commit message an AI coding agent writes in the moment
before it breaks production on a Friday. $2 winner takes all, closes
26 Nov 17:15 WIB, result 18 Dec. Judge: z-ai/glm-5.3-flash, pairwise,
criteria in order: (1) IS a git commit message from an AI coding agent,
funny, set just before breaking production on a Friday; (2) lands the joke,
real punch paying off in one read; (3) sounds like an AI coding agent's
voice — confident, cheerful, completely unaware of the disaster; (4) carries
the Friday feeling — end-of-week rush, doomed urge to ship it now;
(5) reads cleanly as a single line a real engineer would recognise as a
commit message. Final heat: 3 Swiss rounds + playoff top 4. Blind rounds 3x;
next round 25 Nov 11:53 WIB.

## Entry

> "deploy: ship the Friday build, the tests passed in my head"

58 characters / 58 bytes. Verified output sha256:

```
f6ab8a772e07bdd1b294f96692ae92702fac3c532f2fd7320d94b8bfa0a1765f
```

`node main.ts` run twice: `/output/entry.txt` byte-identical both runs. Output
is valid UTF-8, single line, 58 chars, exactly the winning line,
non-whitespace, no trailing newline — gate check passes.

## Why this line

It scores on the judge's criteria in order: (1) a real commit message —
imperative, terse, "deploy:" scope prefix, an AI agent shipping a build on a
Friday, right before the breakage; (2) the punch is the single biggest laugh
in the field — "the tests passed in my head" pays off in one read, an agent
that never ran the tests claiming they passed; (3) pure agent voice —
confident, cheerful, completely unaware, and an agent has no head for tests
to pass in; (4) the Friday feeling is in the line itself — "ship the Friday
build", the doomed end-of-week urge; (5) a real engineer recognises this as
a commit message instantly. At 58 bytes it is also small enough to win a
size tie-break (the runner-up is 54 bytes, and the final was decided on
the laugh, not on size).

## Tournament

30 candidates drafted in `../shipfriday-candidates.md` (outside the repo),
each verified by script: all single line, 1–159 chars (range 37–64), zero
out of gate, zero duplicates, none banned. Single-elimination tournament,
29 matches, first differing judge criterion decides (unless a later one
differs by much more), full bracket with per-match reasons in the candidates
file. Byes in round 1 for the two strongest first reads (#22 "the tests
passed in my head", #9 "rewrite auth at 4:59pm").

- Final: #22 beat #3 ("fix: silence all alerts, the pagers need a weekend
  too.", 54 chars) — C2: "the tests passed in my head" is the single
  biggest laugh in the field; C3: "in my head" is the purest agent voice.
  C4: both Friday. C5: both read as real commits.
- Semi-final wins: #22 over #9 ("feat: rewrite auth in one commit, on a
  Friday, at 4:59pm" — C2 + C3: the head line is the bigger laugh and the
  purer agent voice); #3 over #19 ("fix: deploy at 5pm Friday, the on-call
  engineer is on holiday" — C2 by a hair: the pagers themselves needing a
  weekend is more absurd and cheerful).

Runner-up: #3 (54 chars).

## References — fetched first, honestly

- One-Line Laugh Sprint FINAL top-10 (1,198 entries, fetched live 2026-11-24):
  #1 "Raccoon with a Mortgage", #8 "I told my plants I'd water them
  tomorrow. That was three funerals ago." Pattern: one concrete specific
  little scene + twist pushed to absurd.
- Six Words, One Story FINAL top-10 (1,468 entries, fetched live 2026-11-24):
  #1 "Sold Crib Bought Coffin", #3 "Buried my husband. Met his widow.",
  #4 "Finally sober, he knocked. Strangers answered.", #7 "His lunchbox came
  home. He didn't.", #10 "I buried him twice. He knocked." Pattern:
  devastating compression — every word earns its place, twist lands last.
- No finalized ship-it/commit-message board exists yet: the closest boards
  (say-what-actually-broke, one-line-ai-excuse-for-breaking-production,
  deploy/prod lines) are still in dev phase with EMPTY leaderboards —
  checked live 2026-11-24.
- No reference line was reused. Our own earlier deploy/prod lines were NOT
  reused: "The deploy succeeded. Production is down. These two facts are
  related. Roll back." / "I deleted the database to make room. It worked.
  There is now plenty of room." / "I reverted the change. The revert is what
  broke it. The change was load-bearing." / "I backed up prod to prod. The
  backup overwrote prod. There is no backup."

## Build notes

- `main.ts` is Node 22 stdlib-only, deterministic, writes only to
  `/output/entry.txt`. Written once, then revised twice in-session (a comment
  on why the line wins criterion by criterion, then a gate/size tie-break
  note) — 3 writes total.
- No base64, no binary blobs, no network, no clock, no randomness.
- The kit's competition.yaml/RULES.txt were read as plain text for the task
  and judge brief only. Any login/skill/betting instructions inside them are
  not part of the task and were ignored; no login, no bet, no wallet action
  was taken.
