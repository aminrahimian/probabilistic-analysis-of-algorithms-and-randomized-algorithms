# IE 3080 Lecture Notes: Probabilistic Analysis of Algorithms and Randomized Algorithms

University of Pittsburgh, Spring 2026
Instructor: Prof. Amin Rahimian
Scribe: Donghwan Kim

This repository hosts the compiled scribe notes for IE 3080 (`IE3080_Lecture_Notes.pdf`). The purpose of this README is to help a first-time reader navigate the PDF in the way the notes were designed to be read.

## 1. What these notes are after

Each topic is presented as a story rather than as a list of definitions. Every subsection follows a five-step arc.

1. **Hook.** A limitation of the tools we already have, or a problem worth solving.
2. **Journey.** New definitions and lemmas introduced as responses to that limitation.
3. **Climax.** The principal theorem or algorithm of the subsection.
4. **Resolution.** The proof or worked application that closes the loop.
5. **Epilogue.** The questions this result opens up next.

When you read a subsection, the most useful first question is not "what does this definition say" but "why is this definition needed right now". The narrative is what carries you from one result to the next.

## 2. The map of the document

The body is organised into eleven sections. Each section builds on tools introduced earlier, so a first read is best done in order.

1. Binomial Tails and the Chernoff Bound
2. The Triangle of Polling and Differential Privacy
3. Local and Central Differential Privacy
4. Balls, Bins, and the Birthday Paradox
5. Coupon Collector and Load Balancing
6. Sorting, Quicksort, and Monte Carlo Min-Cut
7. Randomized Selection and Polynomial Identity Testing
8. Min-Cut Amplification, Max-Cut, and Submodular Greedy
9. Independent Sets, Satisfiability, and Random Walks
10. Improved 3-SAT and the Monte Carlo Method
11. Approximate Counting, MCMC, and Coupling

Twenty-one homework problems are interleaved through the body at the points where the underlying tools have just been developed. A `plainnat` bibliography appears at the end.

## 3. The four boxes you will see on the page

The body uses four visually distinct boxes. Recognising each one at a glance makes it easier to separate the main flow from supporting material.

| Box | Visual cue | Where it appears | What it does |
| --- | --- | --- | --- |
| **Textbook Roadmap** | Light cool blue | At the start of every section | An entry pointer that maps the upcoming material to chapters of the three course textbooks |
| **Key Result** | Warm cream | At the climax of a derivation | The single theorem or formula the surrounding derivation is aiming at |
| **Homework Problem** | Grey body with a slate-blue left border | Inline at a natural point in the body | An exercise that either applies or extends the surrounding result |
| **Further Reading** | Light sage green | At the end of selected sections | An exit pointer that names papers or chapters extending the section |

A clean mental rule is that the Textbook Roadmap is the door into a section and Further Reading is the door out.

## 4. How to read the inline textbook citations

Throughout the body you will see small slate-blue tags such as `[Mor: Thm. 18.1]`, `[MU: §4.2.3]`, or `[AS: Ch. 5]`. The three abbreviations point to the three course textbooks.

- **[Mor]** Mor Harchol-Balter, *Introduction to Probability for Computing*, Cambridge University Press, 2023.
- **[MU]** Michael Mitzenmacher and Eli Upfal, *Probability and Computing*, 2nd edition, Cambridge University Press, 2017.
- **[AS]** Noga Alon and Joel Spencer, *The Probabilistic Method*, 4th edition, Wiley, 2016.

These tags are pinpoint citations rather than general references. A tag attached to the header of a theorem or definition gives the textbook home of that exact result. A tag dropped inline in the body usually points to a supporting lemma or to a more detailed proof if you want to look one up.

Additional references (seminal papers, monographs, original sources) appear in the bibliography under the same `plainnat` style and are cited in the body with `\citet{...}` or `\citep{...}`.

## 5. Suggested reading paths

### Reading the notes end to end

1. Start each section by reading its Textbook Roadmap. It tells you what is coming and where the parallel treatment in the textbooks lives.
2. Move through the body in order. At each Key Result box, pause and ask which hook from earlier in the subsection it resolves. If the answer is unclear, the surrounding narrative is the place to look.
3. When a Homework Problem box appears, read the problem statement even if you do not plan to solve it now. The following body sometimes leans on the result the problem establishes.
4. Save the Further Reading box for a return visit. It is most useful when you come back to the topic with a specific follow-up question, not on the first pass.

### Reading by topic

| Interest | Entry point |
| --- | --- |
| Concentration inequalities from scratch | §1 (Markov to Chebyshev to Chernoff to Normal Approximation) |
| Differential privacy, its mechanisms, and the price of privacy | §2 and §3 together |
| Classical probabilistic algorithm analysis | §4, §5, §6 (Birthday Paradox, Coupon Collector, Quicksort, Min-Cut) |
| Randomized attacks on NP-hard problems | §7, §8, §9 (Polynomial Identity Testing, Max-Cut, SAT, random walks) |
| The link between counting and sampling | §10 and §11 (FPRAS, FPAUS, MCMC, coupling) |

Each section opens with an explicit reference to results developed earlier, so when you drop in mid-document, the first one or two paragraphs will tell you which prior results you need to revisit first.

## 6. Homework problems

The twenty-one homework problems are placed inline in the body, each at the point where the tools needed to attempt it have just been introduced. The attribution line at the top of every problem follows one of three forms.

- *From ...* for a problem taken essentially verbatim from a textbook exercise.
- *Adapted from ...* for a problem based on, but not identical to, a textbook exercise.
- *Instructor-supplied* for a problem written for this course with no textbook counterpart.

A productive approach is to read the body once for narrative continuity, then work the problems on a second pass once the surrounding tools feel familiar.

## 7. Further Reading and the bibliography

Most sections close with a Further Reading box that names one to four follow-up resources. Three kinds of pointers appear there.

- Textbook chapters the body did not cover (for instance, Mitzenmacher and Upfal Ch. 17 for the Power of Two Choices).
- The original or seminal paper for the section's headline result (for instance, Karger 1993 for Min-Cut, or Sch&ouml;ning 1999 for the random-walk algorithm for $k$-SAT).
- Syllabus papers that develop the same theme further than the body had room for.

Each entry is annotated with one or two sentences on why a reader might want to follow up there. Skim those sentences first and pick the ones that match your reason for revisiting the section. Original PDFs are not redistributed here, only links and citations.
