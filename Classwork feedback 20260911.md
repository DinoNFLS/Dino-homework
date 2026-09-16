# Classwork feedback 20260911

**Student:** Dino
**Classwork:** Recursion and abstract data types (stack and queue)
**Date:** 2026-09-11

## Score

**85 / 100**

| Question | Score |
|---|---|
| Q1 Recursion (18) | 12 |
| Q2 Recursion in detail (20) | 17 |
| Q3 Stack (20) | 17 |
| Q4 Queue (26) | 23 |
| Q5 Applications (16) | 16 |

## Feedback on incorrect answers

**Q1 (a) definition of recursion (-3 marks)**
- You earn 1 mark for 'a function calls itself', but the key idea is missing: the problem must be reduced to a smaller or simpler version of the same problem, working towards a base case that can be answered directly. 'as the parameter' is also not the right phrase - the function calls itself with a modified argument.

**Q1 (c) why a stack suits recursion (-3 marks)**
- LIFO and the reverse order of unwinding are right. Missing: each call pushes an activation record holding the return address and local variables, and the most recent call is the first to return.

**Q2 (b) winding / unwinding (-3 marks)**
- Both terms are described correctly. Add the mechanism: each call pushes a stack frame, and unwinding pops the frames and combines the results as control returns to the calling statement.

**Q3 (b) stack implementation (-3 marks)**
- 'global' is missing in push() and pop(). In Python, assigning to tp inside a function without 'global tp' creates a local variable and raises UnboundLocalError, so neither method runs. Add 'global tp' to both.

**Q4 (c) circular queue (-3 marks)**
- Wrap-around, full and empty checks are correct. Same issue as Q3(b): 'global rp, fp, length' is missing, so the assignments raise UnboundLocalError.

## Notes (no marks deducted)

**Q1 (b) base case**
- Full marks. Stating that the base case stops the recursion answers the question. To strengthen future answers you could add that it is the simplest instance, solved directly without any further recursive call.

**Q1 (d) factorial trace table**
- Full marks. The question did not specify the starting value, and your trace follows the recursive process correctly down to the base case. Adding the evaluated return values (120, 24, 6, 2, 1) would make the table even stronger.

**Q3 (c) another use of a stack**
- Full marks - the question asked only for a situation, and the browser back button is a valid one. Adding the reason (the most recently visited page is returned to first, LIFO) would complete the answer.

---
_Detailed notes are also added as comments in your Word file._
