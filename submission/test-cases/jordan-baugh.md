# Test Cases: Jordan Baugh

**Team number:** Group 6 v2

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

**Test ID: TC-01**
**Written by: Jordan Baugh**
**Title: Leaderboard Sorting**
**Traces to: app.js -> getRankings()**
**Test type: Unit** (Unit / Integration / System / Acceptance / Boundary Value / Negative / Security)
**Preconditions: The leaderboard must be populated with at least two costumes, and the one that comes first alphabetically has less votes than the other one.**
**Test data: blablabla as Costume name, 0 votes for it. hehehe as costume name, 3 votes for it**

**Steps:**
1. Submit a costume with name as blablabla and don't vote for it
2. Submit a costume with name as hehehe and vote for it 1+ times.
3. Open the leaderboard

---

**Test ID: TC-04**
**Written by: Jordan Baugh**
**Title: Deleting Costumes**
**Traces to: app.js -> deleteCostume()**
**Test type: Security** (Unit / Integration / System / Acceptance / Boundary Value / Negative / Security)
**Preconditions: At least one submitted costume while logged in**
**Test data: A costume called aaaaaa submitted by ghost_gary**

**Steps:**
1. Submit a costume with name as aaaaaa as ghost_gary
2. Log out
3. Navigate to the Gallery page and Delete it

**Expected result: Since aaaaaa was made by ghost_gary it should not be able to be deleted by anyone except ghost_gary**
**Actual result: aaaaaa is deleted without logging in**
**Status: Fail** (Pass / Fail)
**Severity: Critical** (Critical / Major / Minor, Fail only)
**V or V: Verification** (Verification / Validation, Fail only)


