## CS 241: Foundations of Computer Science (Section 006)

### NJIT Spring 2022

**Lecture Times and Location**. 1--2:20pm Tue & Fri in [ECEC 100][]  
**Course Webpage**. [github.com/williamdemeo/cs241-spring2022](https://github.com/williamdemeo/cs241-spring2022)

---

## Syllabus

The *tentative* lecture and homework schedule shown below is subject to change.  Students should return to this page often throughout the semester to keep aprised of any modifications in the schedule or homework due dates.

Below we use the following acronyms:

**DM** = Discrete Mathematics by Johnsonbaugh  
**LP** = [Logic and Proof](https://leanprover.github.io/logic_and_proof/) by Avigad, et al
**ec** = electronic component
**wc** = written component

| **Week** | **Date** | **Topic**                                         | **DM Reading**       | **LP Reading**        | **Homework**                                  |
|----------|----------|---------------------------------------------------|----------------------|-----------------------|-----------------------------------------------|
| **1**    | 18 Jan   | Course overview; Intro to Discrete Math           | §1.1                 | [Ch 1][]              |                                               |
|          | 21 Jan   | Naive set theory; intro to propositional logic    | §1.2, §1.3           | [Ch 11][], [Ch 2][]   | [HW 1 ec][], [HW 1 wc][] due: 2 Feb 10:59pm   |
| **2**    | 25 Jan   | Propositional logic, natural deduction            | §1.4                 | [Ch 3][]              |                                               |
|          | 28 Jan   | First order logic (FOL), quantifiers,             | §1.5, §1.6           | [Ch 7][]              | [HW 2][] due: 9 Feb 10:59pm   |
| **3**    | 1 Feb    | Classical reasoning, proof techniques             | §2.1, §2.2           | [Ch 5][], [Ch 6][]    |                                               |
|          | 4 Feb    | Natural deduction for FOL                         |                      | [Ch 8][]              | | <!--[HW 3 ec][], [HW 3 wc][] due: 16 Feb 10:59pm  | -->
| **4**    | 8 Feb    | Proof by induction                                | §2.4                 | [§17.1][]             |                                               |
|          | 11 Feb   | Strong induction, Well-ordering Principle         | §2.5                 | [§17.2][]             | | <!-- [HW 4][] due: 23 Feb 10:59pm | -->
| **5**    | 15 Feb   | Order relations                                   | §3.3                 | [§13.1][], [§13.2][]  |                                               |
|          | 18 Feb   | Equivalence relations                             | §3.4                 | [§13.3][]             | | <!-- [HW 5][] due: 2 Mar 10:59pm   | -->
| **6**    | 22 Feb   | Functions, sequences                              | §3.1, §3.2           | [Ch 15][]             |                                               |
|          | 25 Feb   | Properties of functions                           |                      | [§15.2][]             | |
| **7**    | 1 Mar    | Analysis of algorithms                            | §4.3                 |                       | |
|          | 4 Mar    | Recursive algorithms                              | §4.4                 |                       | |
| **8**    | 8 Mar    | Midterm Exam (coverage: weeks 1--6)               |                      |                       | |
|          | 11 Mar   |  |  |  | |
| **9**    | 15 Mar   |  |  |  | |
|          | 18 Mar   |  |  |  | |
| **10**   | 22 Mar   |  |  |  | |
|          | 25 Mar   |  |  |  | |
| **11**   | 29 Mar   |  |  |  | |
|          | 1 Apr    |  |  |  | |
| **12**   | 5 Apr    |  |  |  | |
|          | 8 Apr    |  |  |  | |
| **13**   | 12 Apr   |  |  |  | |
|          | 15 Apr   |  |  |  | |
| **14**   | 19 Apr   |  |  |  | |
|          | 22 Apr   |  |  |  | |
| **15**   | 26 Apr   |  |  |  | |
|          | 29 Apr   |  |  |  | |
| **16**   | 3 May    | Review (last class)  |                 |                        | |
|          | 4 May    | (reading day)        |                 |                        | |
|          | 6 May    | (reading day)        |                 |                        | |
|          | 6 May    | (final exams begin)  |                 |                        | |
|          | 12 May   | (final exams end)    |                 |                        | |
|          | 14 May   | (final grades due)   |                 |                        | |



[ECEC 100]: https://goo.gl/maps/ZBW1fdPqii6frCJZ7


[Ch 1]: https://leanprover.github.io/logic_and_proof/introduction.html
[Ch 2]: https://leanprover.github.io/logic_and_proof/propositional_logic.html
[Ch 3]: https://leanprover.github.io/logic_and_proof/natural_deduction_for_propositional_logic.html
[Ch 5]: https://leanprover.github.io/logic_and_proof/classical_reasoning.html
[Ch 6]: https://leanprover.github.io/logic_and_proof/semantics_of_propositional_logic.html
[Ch 7]: https://leanprover.github.io/logic_and_proof/first_order_logic.html
[Ch 8]: https://leanprover.github.io/logic_and_proof/natural_deduction_for_first_order_logic.html
[Ch 10]: https://leanprover.github.io/logic_and_proof/semantics_of_first_order_logic.html
[Ch 11]: https://leanprover.github.io/logic_and_proof/sets.html
[Ch 13]: https://leanprover.github.io/logic_and_proof/relations.html
[§13.1]: https://leanprover.github.io/logic_and_proof/relations.html
[§13.2]: https://leanprover.github.io/logic_and_proof/relations.html#more-on-orderings
[§13.3]: https://leanprover.github.io/logic_and_proof/relations.html#equivalence-relations-and-equality
[Ch 15]: https://leanprover.github.io/logic_and_proof/functions.html
[§15.2]: https://leanprover.github.io/logic_and_proof/functions.html#injective-surjective-and-bijective-functions
[Ch 17]: https://leanprover.github.io/logic_and_proof/the_natural_numbers_and_induction.html
[§17.1]: https://leanprover.github.io/logic_and_proof/the_natural_numbers_and_induction.html
[§17.2]: https://leanprover.github.io/logic_and_proof/the_natural_numbers_and_induction.html#variants-of-induction
[Ch 20]: https://leanprover.github.io/logic_and_proof/combinatorics.html
[gradescope]: https://www.gradescope.com/courses/360140/assignments

[HW 1 ec]: https://www.gradescope.com/courses/360140/assignments
[HW 2 ec]: https://www.gradescope.com/courses/360140/assignments
[HW 3 ec]: https://www.gradescope.com/courses/360140/assignments
[HW 4 ec]: https://www.gradescope.com/courses/360140/assignments
[HW 5 ec]: https://www.gradescope.com/courses/360140/assignments
[HW 6 ec]: https://www.gradescope.com/courses/360140/assignments
[HW 7 ec]: https://www.gradescope.com/courses/360140/assignments
[HW 8 ec]: https://www.gradescope.com/courses/360140/assignments
[HW 9 ec]: https://www.gradescope.com/courses/360140/assignments

[HW 1 wc]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw01-wc.pdf
[HW 2]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw02.pdf
[HW 3 wc]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw03-wc.pdf
[HW 4 wc]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw04-wc.pdf
[HW 5 wc]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw05-wc.pdf
[HW 6 wc]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw06-wc.pdf
[HW 7 wc]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw07-wc.pdf
[HW 8 wc]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw08-wc.pdf
[HW 9 wc]: https://github.com/williamdemeo/cs241-spring2022/raw/master/homework/hw09-wc.pdf
