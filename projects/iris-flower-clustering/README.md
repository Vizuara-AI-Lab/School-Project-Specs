# Project Name: Iris Flower Clustering (K-Means)

## Issues

### 1. Weak Framing of the ML Problem

The module opens with a narrative-heavy description but fails to clearly establish:

* what is known vs unknown in the problem
* why this is an *unsupervised* learning task
* what K-Means is expected to do and what it cannot do

As a result, students may enjoy the story but not understand the nature of the ML task they are performing.

---

### 2. Overly Passive, Text-Driven Learning Experience

Large blocks of explanatory text dominate the module, with minimal interaction.
Key ML concepts such as clustering, distance, and similarity are explained verbally rather than demonstrated.

This makes the learning experience closer to reading an article than *doing machine learning*.

---

### 3. Concept Navigation Exists but Lacks Pedagogical Clarity

The sidebar shows “Concept 0–4” (Problem Scoping, Data Acquisition, etc.), but:

* concepts feel isolated rather than sequential
* learning objectives are not explicit
* locked concepts feel arbitrary instead of earned

Students do not feel a sense of conceptual progression or mastery.

---

### 4. Decorative Visuals Replace Instructional Visuals

Large, AI-generated illustrations are visually appealing but:

* do not encode any data or ML insight
* take up significant screen space
* distract from the core learning task

These visuals add aesthetic value but little educational value.

---

### 5. Absence of Core K-Means Visualizations

Despite being a clustering module:

* no scatter plots are prominently visible
* clusters are not shown as colored groups
* centroids and distance-based assignments are not visualized

This undermines the geometric intuition that is central to understanding K-Means.

---

### 6. Modeling Step Is Abstracted Away

Students are not meaningfully involved in:

* choosing the value of *k*
* observing centroid initialization
* seeing iterative reassignment and convergence

The algorithm appears to “just run,” reinforcing a black-box view of ML.

---

### 7. Misaligned Evaluation and Quizzes

The QnA section includes questions about biological facts (e.g., sepals and petals) rather than:

* clustering behavior
* limitations of K-Means
* interpretation of visual results

Assessment currently tests domain trivia instead of ML understanding.

---

### 8. Lack of Exploration, Prediction, and Feedback

Students are rarely asked to:

* make predictions before seeing results
* experiment with different feature combinations
* reflect on why outcomes change

Without exploration and feedback, conceptual learning remains shallow.

---

## Goals

* Design the module specifically to teach **unsupervised learning and clustering intuition** rather than dataset trivia
* Clearly frame the Iris problem as one where labels are unknown and structure must be *discovered*
* Replace passive reading with interactive exploration wherever possible
* Treat visualization as the **primary teaching medium**, not a secondary output
* Reduce decorative visuals that do not directly support learning
* Establish a clear, linear-yet-flexible progression from problem framing to evaluation
* Make each concept feel like a meaningful milestone with explicit learning outcomes
* Allow students to directly manipulate:

  * feature selection (sepal vs petal)
  * number of clusters (*k*)
  * clustering runs
* Visually demonstrate:

  * distance-based assignment
  * centroid movement
  * convergence over iterations
* Ensure students understand that clustering results can change based on choices and assumptions
* Redesign quizzes to assess ML reasoning, not biological memorization
* Encourage prediction, experimentation, and reflection as part of the learning loop
* Keep the tone suitable for high school students: exploratory, curious, and serious without feeling academic or dull
* Maintain a clean, intentional visual language that avoids excessive gradients, emojis, and auto-generated aesthetics
* Introduce progress tracking subtly, focusing on conceptual mastery rather than completion
* Ensure students cannot advance without interacting meaningfully with each concept
* **You are encouraged to experiment with UI, UX, structure, and interaction patterns as long as the primary objective of helping students build intuition for K-Means clustering is achieved**

---

## High-Level Implementation Guidance (For the Developer)

* Think in terms of **“show, then explain”**, not the other way around
* Every major visual should answer: *What is changing, and why does it matter?*
* Prefer small, focused interactions over long explanations
* Assume the student has never seen clustering before, but is capable of reasoning visually
* If a section can be understood without reading any text, it’s probably well-designed
