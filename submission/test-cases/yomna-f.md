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

**Test ID:**
**Written by:**
**Title:**
**Traces to:**
**Test type:**
**Preconditions:**
**Test data:**

**Steps:**
1.
2.
3.

**Expected result:**
**Actual result:**
**Status:**
**Severity:**
**V or V:**

---
