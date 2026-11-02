# Task 1 - AI Output

- **Name:** Ben Coppage
- **AI tool and model:** Claude Opus 5.5 (Anthropic)
- **Date and time prompted:** 2026-11-02, started 1:29 p.m. CT, usable answer at 1:30 p.m. CT
- **Data provenance:** `ai/workshops_spring2026.csv` is a synthetic dataset created for i.c.stars Tech Foundations Performance Assessment C (Week 9), November 2026. The "Neighborhood Tech Hub," its workshops, and every name and email address in the file are fictional.
- **Columns I removed before prompting (privacy):** host_name, host_email

## Prompt I used (copy it exactly)

```text
ROLE: You are a data analyst for a community nonprofit.

CONTEXT: The data below is a synthetic dataset created for i.c.stars Tech Foundations Performance Assessment C (Week 9), November 2026. It lists 24 free digital-skills workshops run by the fictional "Neighborhood Tech Hub" in six Chicago neighborhoods from March to May 2026. Personal information has been removed.

TASK: Write a summary of this dataset for the nonprofit's program director in 120-180 words.

INCLUDE: totals and the overall attendance rate; the best and worst results; the main patterns in the data; one recommendation.

RULES: Use only numbers you can calculate from the data. Say so if something can't be determined from the data.

FORMAT: Short paragraphs, no bullet points.

DATA:
workshop_id,date,neighborhood,topic,time_slot,registered,attended,avg_rating,followup_signups
W01,2026-03-03,Englewood,Online Job Search,Weekday 10am,22,12,4.7,5
W02,2026-03-05,Rogers Park,Online Job Search,Weekday 6pm,18,15,4.4,6
W03,2026-03-07,Logan Square,Intro to Spreadsheets,Saturday 11am,19,17,4.2,4
W04,2026-03-12,Englewood,Smartphone Essentials,Weekday 6pm,27,21,4.5,3
W05,2026-03-14,Pilsen,Online Job Search,Saturday 11am,24,21,4.6,8
W06,2026-03-18,Pilsen,Online Safety Basics,Weekday 6pm,23,18,4.5,3
W07,2026-03-21,Bronzeville,Smartphone Essentials,Saturday 11am,24,20,4.4,3
W08,2026-03-25,Logan Square,Online Job Search,Weekday 6pm,23,19,4.7,7
W09,2026-04-01,Bronzeville,Intro to Spreadsheets,Weekday 6pm,16,13,4.4,3
W10,2026-04-04,Rogers Park,Smartphone Essentials,Saturday 11am,24,21,4.3,4
W11,2026-04-07,Logan Square,Smartphone Essentials,Weekday 6pm,24,18,4.3,4
W12,2026-04-11,Austin,Intro to Spreadsheets,Saturday 11am,19,16,4.0,3
W13,2026-04-14,Pilsen,Smartphone Essentials,Weekday 10am,20,11,4.6,2
W14,2026-04-16,Bronzeville,Online Safety Basics,Weekday 10am,21,12,4.6,2
W15,2026-04-23,Pilsen,Intro to Spreadsheets,Weekday 6pm,24,19,3.9,4
W16,2026-04-25,Rogers Park,Intro to Spreadsheets,Saturday 11am,16,14,4.3,2
W17,2026-04-30,Austin,Online Safety Basics,Weekday 10am,17,9,4.4,1
W18,2026-05-02,Logan Square,Online Safety Basics,Saturday 11am,20,18,4.6,4
W19,2026-05-06,Englewood,Intro to Spreadsheets,Weekday 10am,23,13,4.0,2
W20,2026-05-13,Austin,Online Job Search,Weekday 6pm,27,21,4.6,8
W21,2026-05-16,Bronzeville,Online Job Search,Saturday 11am,23,19,4.9,7
W22,2026-05-19,Austin,Smartphone Essentials,Weekday 10am,25,14,4.4,2
W23,2026-05-23,Englewood,Online Safety Basics,Saturday 11am,21,18,4.6,3
W24,2026-05-26,Rogers Park,Online Safety Basics,Weekday 6pm,18,15,4.3,3
```

## AI output (copy it exactly; do not fix anything here)

Neighborhood Tech Hub ran 24 workshops in six neighborhoods from March to May 2026. 518 people registered and 394 attended, for a 76.1% attendance rate. Attendees made 93 follow-up signups.
W18 (Online Safety Basics, Logan Square) had the best attendance at 90.0%. W17 (Online Safety Basics, Austin) had the worst at 52.9%. W21 (Online Job Search, Bronzeville) had the top rating, 4.9. W15 (Intro to Spreadsheets, Pilsen) had the lowest, 3.9.
Time slot drove attendance. Saturday 11am sessions reached 86.3% and weekday 6pm sessions reached 79.5%. Weekday 10am sessions reached only 55.5%, and they were the six lowest-attended workshops.
Online Job Search had the strongest results. Its six sessions averaged a 4.65 rating and produced 41 of the 93 follow-up signups. Intro to Spreadsheets averaged the lowest rating, 4.13.
The data does not show why registrants missed sessions or whether the same people attended more than one workshop.
Recommendation: move weekday 10am workshops to Saturday 11am or weekday 6pm.
