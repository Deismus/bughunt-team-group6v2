# Test Cases: Yomna F

**Team number:** [XX]

<!--
HOW TO USE THIS FILE
1. Copy this file. Name the copy with your first name and last initial, like  maria-g.md
2. Leave TEMPLATE.md untouched for your teammates.
3. Write at least ONE failing test case. More is better.
4. Copy the block between the lines for each new test case.
5. Test IDs: use your initials plus a number, like  MG-01, MG-02. This keeps IDs unique across your team.
6. See docs/TESTING_FIELD_GUIDE.md for the sample test case TC-00.
-->

---

**Test ID:** TC-2
**Written by:** Yomna F
**Title:** Votes remaining goes to -1 and a 4th vote is accepted after the 3-vote limit
**Traces to:** REQ-09
**Test type:** Boundary Value
**Preconditions:** pp is running at profmanjupriya.github.io/fright-night-bug-hunt/app/.
**Test data:** User ghost_gary; 3 votes available; 4 clicks on a "Vote" button 

**Steps:**
1. Log in and open the Vote tab
2. Click "Vote" 3 times. Check that "Votes remaining" goes 2, 1, 0.
3. Click "Vote" a 4th time 


**Expected result:** At 0 votes remaining, the 4th click is rejected.
**Actual result:** The message "You have used all of your votes!" appears but "Votes remaining" drops to -1 and the costume's vote count increases.
**Severity:** Major
**V or V:** Verification
---

**Test ID:** TC-4
**Written by:** Yomna F
**Title:** Voting deadline countdown ends around 5:00 PM on Oct 31 instead of midnight
**Traces to:** REQ-13 (Voting closes at midnight on October 31)
**Test type:** Boundary Value
**Preconditions:** App is running at profmanjupriya.github.io/fright-night-bug-hunt/app/. Logged in as ghost_gary. Current date/time is known (Oct 29, 2026, 2:55 PM local time).
**Test data:** Countdown banner in the header; local time of the test machine (San Diego, Pacific time)

**Steps:**
1. Log in as ghost_gary and note the current local date and time.
2. Read the "Voting closes in ..." countdown in the top right of the header.
3. Add the countdown (2d 2h 4m) to the current local time to get the closing time.
4. Compare the result with the deadline in REQ-13 (midnight on October 31).

**Expected result:** The countdown ends at midnight on October 31. On Oct 29 at 2:55 PM it should show about 2d 9h 5m (or 1d 9h 5m, depending on whether "midnight on October 31" means the start or the end of that day).
**Actual result:** The countdown shows 2d 2h 4m, so voting closes around 5:00 PM on October 31, about 7 hours before midnight.
**Status:** Fail
**Severity:** Major
**V or V:** Verification

---
