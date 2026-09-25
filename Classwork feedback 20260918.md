# Classwork feedback 20260918

**Student:** Dino
**Classwork:** Abstract data types - binary tree, linked list, circular queue
**Date:** 2026-09-18

## Score

**94 / 100**

| Question | Score |
|---|---|
| Q1 Binary tree concepts (25) | 22 |
| Q2 Linked list (35) | 34 |
| Q3 Circular queue programming (40) | 38 |

## Feedback on incorrect answers

**Q1 (c) subtree (-1 mark)**
- Your example (node 25 with 16 and 32) is correct and the nodes are named, which earns two marks. One is lost on the definition: a subtree is a node together with all of its **descendants**, not just its children - "descendants" includes every node in the branches below, however deep they go.

**Q1 (f) choice of key (-2 marks)**
- Uniqueness, the fact that surnames can be duplicated, and the one-to-one mapping point are all credited. Missing: that a key must also be comparable, which is what lets the tree order and search by it; and a closing statement that ties the two together.

**Q2 (e) returning a node to the heap (-1 mark)**
- Updating `heapStartPointer` to the removed node, and the fact that the node can then be reused, are both credited. Missing: the removed node's own pointer is set to the **old** `heapStartPointer` first, so that it links on to the rest of the free list, and only then is `heapStartPointer` moved onto it.

**Q3 (a) declarations (-1 mark)**
- The list of 8 items and `orderCount = 0` are correct. The question asks for `front`, `rear` and `orderCount` **all** to be initialised to 0, and you set `rear` to -1. Your own wrap-around makes that work, so the logic is sound, but it is not what the question specified.

**Q3 (f) three further dequeue calls (-1 mark)**
- The empty queue and the repeated "EMPTY" returns are correct, and stating that `orderCount = 0` earns the explanation marks. The final mark is for linking it to the code: `dequeue()` tests `orderCount == 0` and returns "EMPTY" **before** it reads the list, so the pointers are never touched.

## Notes (no marks deducted)

**Q1 (b) level and height**
- Full marks. Level 3 and depth 2 are both correct. To make the answer complete in the exam it also helps to state that the root is counted as level 1, which is what makes 45 level 3, and to define height as the number of edges on the longest path from the root to the deepest leaf.

**Q1 (d) binary search tree rule**
- Full marks. Both rules are correctly stated. Since duplicate keys do not appear in A-Level or IB binary search tree questions, "greater than" for the right child is accepted on its own. The fuller wording you may see in a mark scheme is "greater than or equal to", which is the convention when duplicates are allowed.

**Q1 (e) inserting 40**
- Full marks. Your answer - 45, left child - is correct, and the three comparisons are right.

**Q2 (a) trace table**
- Full marks. Every itemPointer is correct, and `-1` in the last row is the right value: the node holding 61 is the last node in the list, so its next pointer is the null pointer. It is worth adding in words that the search stops and returns the index once the item is found.

**Q3 (b), (c), (d), (e) implementation**
- Full marks. The enqueue, dequeue, main program and screenshot are all correct and the output appears in the right order.

---
_Detailed notes are also added as comments in your Word file._
