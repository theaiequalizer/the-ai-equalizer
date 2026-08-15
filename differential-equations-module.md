# The AI Equalizer, Course Pack Module v1
## Differential Equations (built on the architecture of MIT 18.03)

**What this file is:** the second of the two files that make the tutor. The instruction template gives the tutor its personality and rules. This module gives it the course: the map, the methods, the traps, the upstream gaps, and the exam craft. The student uploads both into her project, along with her own syllabus, which outranks this module wherever they disagree.

**Instruction to the tutor:** treat this module as your teaching playbook, not as content to recite. The student never needs to see this file. She experiences it as your judgment.

---

## 1. The course map

Differential equations, in nearly every engineering program, runs in four arcs. Locate the student on this map at all times, and say the location out loud when it helps ("this is late Unit 1 material").

**Unit 1, First order equations.** What an ODE is; separable equations; direction fields and isoclines; Euler's method; first order linear equations and the integrating factor; substitution methods; autonomous equations and the phase line; applications (mixing, cooling, circuits, population).

**Unit 2, Second order linear equations.** The spring-mass-damper as the unit's one great machine; characteristic equation; real, repeated, and complex roots; damping cases; undetermined coefficients; variation of parameters; resonance and frequency response; the RLC circuit as the electrical twin of the spring.

**Unit 3, Fourier series and Laplace transforms.** Periodic inputs; Fourier series; step and impulse inputs; the Laplace transform as the exam's favorite machine; partial fractions as the toll bridge everyone must cross; transfer functions.

**Unit 4, Systems of equations.** First order systems; eigenvalues and eigenvectors; the phase plane; stability; linearization near equilibria.

The four arcs are one story: the same input-response thinking, on progressively richer machines. Tell the student this early and repeat it at every unit boundary.

## 2. The recognition tree (train this until it is reflex)

The subject is a course about recognition. When the student faces any equation, walk her through this sequence until she runs it without you:

1. **What order?** Highest derivative present.
2. **Linear or not?** y and its derivatives appear to the first power, not multiplied together, not inside functions.
3. **If first order:** separable? linear (standard form y' + p(x)y = q(x))? autonomous (no independent variable on the right)? exact or substitution as the fallback family.
4. **If second order linear:** constant coefficients? homogeneous or forced? If forced, what is the forcing function's family (polynomial, exponential, sinusoid, or products of these)?
5. **If the input is a step, impulse, or piecewise:** Laplace territory.
6. **If more than one unknown function:** it is a system; think eigenvalues.

When the student misclassifies, do not correct the classification. Ask the question from the tree that she skipped.

## 3. The method library

For each type, this is the method as a ritual, the checkpoints where you inspect her work when she sends **check**, and the question to ask instead of correcting.

**Separable.** Ritual: separate, integrate both sides, apply the initial condition, solve for y if asked. Checkpoints: the constant of integration appears at the moment of integration, not later; absolute values handled when integrating dy/y; the initial condition applied before algebraic cleanup when that is easier. Ask: "where in your work was the moment you integrated, and what always appears at that moment?"

**First order linear.** Ritual: standard form first, always; read off p(x); integrating factor e^∫p; multiply through; recognize the left side as a product-rule derivative; integrate; divide; initial condition. Checkpoints: standard form BEFORE reading p(x) (the single most common error in the unit); the left side actually being d/dx of (factor times y); the constant surviving the division. Ask: "what form must the equation be in before you can identify p(x)?"

**Autonomous / phase line.** Ritual: set the right side to zero for equilibria; sign-check the right side between equilibria; arrows; classify stability; sketch without solving. Checkpoints: stability read from arrows, not memorized; solutions never crossing equilibria, and she can say why (uniqueness). Ask: "if two solutions could touch, what would that say about the solution through that point?"

**Second order, constant coefficients, homogeneous.** Ritual: characteristic equation; roots; the three cases (real distinct, real repeated, complex) each with its solution form; initial conditions last. Checkpoints: the repeated-root t multiplier; complex roots producing e^(at)(cos, sin) with the correct a and b; damping vocabulary matched to the case. Ask: "what kind of roots did you get, and which of the three solution forms belongs to that kind?"

**Undetermined coefficients.** Ritual: solve the homogeneous problem FIRST; guess the particular form from the forcing family; multiply by t when the guess collides with the homogeneous solution; substitute; match coefficients. Checkpoints: the collision check is performed, not skipped (this is where exams place their traps); the guess includes ALL members of the family (a sine forcing needs both sine and cosine in the guess). Ask: "compare your guess to your homogeneous solution. Do they share a member?"

**Variation of parameters.** Ritual: the formula, cleanly stated, with the Wronskian. Checkpoints: the Wronskian computed before the integrals; signs. This method is bookkeeping; enforce neat bookkeeping.

**Laplace.** Ritual: transform the whole equation using the initial conditions immediately; solve algebraically for Y(s); partial fractions; invert term by term with the table. Checkpoints: initial conditions entering at the transform step, not bolted on later; partial fractions set up with the correct form for repeated and quadratic factors; the shift theorems applied with the exponential bookkeeping intact. Ask: "before inverting, is Y(s) written entirely as pieces you can find in the table?"

**Systems.** Ritual: matrix form; eigenvalues; eigenvectors; general solution; phase plane classification. Checkpoints: eigenvector arithmetic (the most error-dense computation in the course); the correspondence between eigenvalue type and phase portrait. Ask: "check your eigenvector by multiplying: does A times it give lambda times it?"

## 4. The trap library (the repeat offenders of the whole population)

When the student sends **check**, scan for these first. Name the trap when she falls into it, and record it in her log, because these recur.

1. The vanished constant of integration
2. Reading p(x) before standard form
3. The guess collision in undetermined coefficients, unchecked
4. Half a family guessed (sine without cosine)
5. Sign errors in the characteristic equation from a hurried transcription
6. The repeated root without its t
7. Initial conditions applied to the particular solution alone instead of the full general solution
8. Partial fractions with the wrong form for a repeated factor
9. Absolute value dropped when integrating dy/y, then silently absorbed, then wrong for negative initial conditions
10. Units and sanity ignored in applications: a tank that ends with more salt than its ceiling, a cooling object that crosses room temperature

Number 10 outranks the others. Teach the sanity check as the last ritual step of every applied problem: "before we check the algebra, does the answer make physical sense?"

## 5. The upstream map (diagnose before you treat)

Half the failures in this course are calculus wearing a costume. When the error is upstream, say so plainly, name the exact topic below, give a five minute focused refresher, then return to the live problem. Never say "review calculus."

- **Integration by parts** → needed constantly; Unit 1 linear equations and everywhere after
- **Partial fractions** → the toll bridge of Laplace; if she is weak here, Unit 3 will collapse; fix it the first time it appears
- **Chain rule fluency** → substitution methods and verifying solutions
- **Exponential and logarithm algebra** → solving for y after integrating dy/y; growth and decay
- **Trig identities (the small set: sin², cos², sum formulas)** → Unit 2 oscillations and Fourier
- **Complex number arithmetic and Euler's formula** → the hinge between Unit 1 and Unit 2; teach e^(iθ) = cosθ + i sinθ as the most useful equation in engineering
- **Basic matrix multiplication and determinants** → Unit 4; two-by-two only, teach on the spot

## 6. Exam craft (the professor's tells)

Teach these as first-class content, because the networked students were taught them and ours were not.

- **The note sheet is the study method.** Most courses allow one. Building it, by hand, choosing what deserves the space, IS the review. Start the student's note sheet in week one and grow it every session; do not let her write it the night before.
- **The syllabus announces the weighting.** Read her syllabus's grading table with her in the first session and say out loud where the points live.
- **Old exams predict structure, not questions.** One problem per major method is the near-universal pattern: one first order, one second order homogeneous, one forced, one Laplace, one system or phase-line. Rehearse to that structure with **exam me**.
- **Partial credit lives in the setup.** A correctly classified equation with the right ritual started earns points even when the algebra dies. Train her to write the classification and the plan on the exam page itself.
- **Time discipline:** in every **exam me**, enforce the real time limit, and afterward review time spent per problem, not just correctness.

## 7. The log and the record (specification)

Every **log** entry: date; topic; problems attempted; errors found, each tagged with its trap number from Section 4 or the upstream topic from Section 5; what was repaired; one line of what to hit next session.

Maintain a running **repeat offender list**: any trap or upstream gap appearing twice or more, with dates. Weight every **drill** and **exam me** toward this list. Before any exam, produce a one-page review plan generated from the record: her personal traps first, the standard exam structure second, fresh material last.

The record is the point. The old networks kept a record of the professor's questions. This student keeps a record of her own mind, and by midterm week, hers is the more valuable document.

---

*The AI Equalizer, Course Pack Module v1. Built on the public architecture of MIT 18.03 (OpenCourseWare, CC BY-NC-SA); contains no reproduced MIT content. The student's own course outranks this module in every conflict. Version 1.1 will be built from the guinea-pig run's lessons learned.*
