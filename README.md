## Academics: Scheduling a help room, for math, physics, or writing, with TAs/instructors. We may add a feature for scheduling teaching assignments as well. I have a feeling that a teaching schedule is easier with marriage perposal algorithm (Gale–Shapley algorithm ). We need to investigate that.

We know at least two sets of codes need to be written.

## Set 1:

Ask the user (the manager or supervisor) a few questions so the nature of the scheduling becomes apparent to us. Then use the user's answers to create surveys for TAs to rate every time slot according to their preference and rate if they want back to back assignments.

Questions: 
(1) Are you creating a repeating weekly schedule? (2) What is the time interval length you wish to schedule each TA? The answer has to be reasonable, so give two options: 30 minutes or 1 hour. If the answer to (1) is yes, create a grid with days of the week as rows and the columns are all of the time slots of the length provided in (2) in a day starting at midnight. Assign an array to this grid so you can create a schedule later and ask: (3) Choose all time slots that you need to schedule and the number of TAs needed.

If the answer to (1) is no, ask (4) What year are you planning to schedule? Then make a calendar with 12 months of the year in (4) in 12 grids. Assign a matrix that corresponds to this grid and ask: (5) Choose all dates that you need to schedule and the number of TAs needed. Then create a grid with time intervals using (2) and the answers in (5). 
Ask the user: (6) Do you prefer to survey your students with Google Forms or Microsoft Forms? (7) Upload a list of the TAs with their email addresses and the maximum number of hours that can be assigned to them.(8) How many TAs need to work in each time slot?
(9) Do you have more experienced TAs who need to be assigned to special time slots?

If the answer is yes, ask:
Upload a list of more experienced TAs and choose the time slots that need more experienced TAs. Take the user's answers in (10) in a grid that is created from their answers in (3) or (5). Create the form that is chosen in (6), and give options to rate each time slot by 0-4 chosen in either (3) or (5). These forms will contain exact instructions.

_______________________________________________________________________________________________________________________________________________________________________________________________________________________________
## Set 2:

Use the data from Set 1.
Set up a linear programming problem with a set of binary variables for each TA, $x_1, x_2,...,x_n$ that correspond to each time slot assigned in (3) and (5).

Constraints:
* (A) Each TA’s average schedule rate should be ≥ 2. (This needs a bit of pondering because we want to include some back to back assignment rating.)

* (B) The number of TAs in each time slot should be ≥ the minimum number of TAs needed for that time slot. This number can differe by how busy the help room is during the different hours of the day. 

* (C) The number of hours assigned to each TA should be  ≤  than the maximum number that can be assigned to them. This can vary from TA to TA according to their contract and responsibilities.

Give the result in a table for the user.
_______________________________________________________________________________________________________________________________________________________________________________________________________________________________

[Back to top](#readme)
