# Task 1 - AI Evaluation Log

Compare the AI output (`ai_output.md`) with the human baseline (`baseline_summary.md`).
Use **at least two** criteria. Fill one row per criterion you use, and give evidence: quote numbers or phrases.

| Criterion | What the baseline says | What the AI says | Match? (Yes / Partly / No) | Evidence and notes |
| --- | --- | --- | --- | --- |
| Accuracy (numbers and facts) | 518 registered, 394 attended, 76%. Weekday 10am 55%, weekday 6pm 80%, Saturday 11am 86%. Online Job Search: 41 of 93 sign-ups. | 518 registered, 394 attended, 76.1%. Weekday 10am 55.5%, weekday 6pm 79.5%, Saturday 11am 86.3%. Online Job Search: 41 of 93 sign-ups. | Yes | Every number matches the baseline after rounding. I checked them against the CSV. Extra AI facts are also correct: W18 best at 90.0% (18/20), W17 worst at 52.9% (9/17), Online Job Search average rating 4.65. |
| Completeness (key points covered) | Austin (68%) and Englewood (69%) were lowest, but hosted 4 of the 6 morning sessions; outside mornings they reached 80-81%. Average rating 4.4 (range 3.9 to 4.9). | No neighborhood results at all. Gives the top (4.9) and bottom (3.9) session ratings, but no overall average. | Partly | Missed the most important insight: the low neighborhoods are explained by the morning time slot. Also missed one limit: ratings only come from attendees who stayed to the end. |
| Bias or privacy risk | Warns: fix morning sessions "before drawing any conclusion about interest in a particular neighborhood." | Recommends moving morning sessions, with no warning about neighborhoods. | Partly | No PII in the prompt: host_name and host_email removed. Risk: without the neighborhood context, a reader could later see low Austin and Englewood numbers and blame the communities instead of the time slot. |
| Reliability (would you trust it without checking?) | Numbers checked by hand by program staff. | Numbers correct, but key context left out. | Partly | I would not use it without checking. The math was right this time, but I only knew that after checking against the CSV. It also chose what to leave out without saying so. |
| Time saved (estimate in minutes) | Written by hand; I estimate about 25 minutes. | Usable answer in 1 minute (1:29 to 1:30 p.m.), plus about 10 minutes to check it. | Yes | About 14 minutes saved. Checking time cuts into the savings. |

## Gaps or risks I found (at least one)

1. The AI did not report attendance by neighborhood. It missed that Austin and Englewood look weak only because they hosted 4 of the 6 morning sessions. This could lead to unfair conclusions about those neighborhoods.
2. No overall average rating (4.4), and it left out the limit that ratings come only from attendees who stayed to the end.

## Decision (check one)

- [ ] **Accept** as is
- [x] **Edit** (fix it, then use it)
- [ ] **Reject** (don't use it)

## Why I decided this (3-5 sentences)

Every number in the AI summary was correct when I checked it against the CSV and the baseline. The time slot pattern and the recommendation match the baseline. But the AI left out the neighborhood results and the fact that the morning slot explains Austin's and Englewood's low attendance. Without that, a reader could wrongly blame those neighborhoods. The summary is worth keeping, but it needs the missing context added before a program director uses it.

## If you chose Edit: corrected summary (optional)

From March 3 to May 26, 2026, Neighborhood Tech Hub ran 24 free workshops, four in each of six Chicago neighborhoods. 518 people registered and 394 attended, a 76% attendance rate.

Time slot drove attendance. Saturday 11am sessions reached 86% and weekday 6pm sessions 80%. Weekday 10am sessions reached only 55%, and they were the six lowest-attended workshops.

Austin (68%) and Englewood (69%) had the lowest overall attendance, but they hosted four of the six morning sessions. Outside the morning slot, they reached 80-81%, in line with the other neighborhoods.

Attendees rated the workshops 4.4 out of 5 on average (range 3.9 to 4.9). Online Job Search had the best results: a 4.65 average rating and 41 of the 93 follow-up sign-ups.

Limits: one season of data; ratings come only from attendees who stayed to the end; the data cannot show duplicate registrations or why people missed sessions.

Recommendation: move weekday 10am sessions to evenings or Saturdays before drawing conclusions about any neighborhood.
