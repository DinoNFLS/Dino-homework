# Classwork feedback 20260904

**Student:** Dino
**Classwork:** Algorithms - Big-O, linear search, binary search, insertion sort
**Date:** 2026-09-04

## Score

**93 / 100**

| Question | Score |
|---|---|
| Q1 | 28/30 |
| Q2 | 39/40 |
| Q3 | 26/30 |

## Feedback on incorrect answers

**Q1 (a)(iii) (-1 mark)**
- Briefer explanation than required - should state that when the target is missing, found never becomes True and the else branch returns -1 regardless of i.

**Q1 (d) (-2 marks)**
- Correct that -1 is returned, but gave no reason WHY the empty-list test is valid (a boundary case that can reveal index / return-value errors).

**Q2 (d) (-1 mark)**
- 4 comparisons correct, but the halving mechanism (10 -> 5 -> 2 -> 1) was not explained - 'O(log n)' alone is too brief.

**Q3 (a) (-3 marks)**
- while condition written as 'current < values[pos-1] and pos > 0' - when pos reaches 0, values[pos-1] is evaluated first, giving the negative index values[-1]. This is a real bug, not just style.

**Q3 (b) (-1 mark)**
- Same while-condition ordering issue carried over from part (a).

---
_Detailed notes are also added as comments in your Word file._
