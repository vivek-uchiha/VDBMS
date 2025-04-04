## Query Processing in a Vector Database Management System !

- Query processing in a **Vector Database Management System (VDBMS)** begins with a **search specification**.
- The search specification includes:
  - The **similarity score** (used to measure how close vectors are).
  - The **query type** (e.g., nearest neighbor search).
- **Search criteria** are passed into the system via a **query interface**.
- Once the query is received by the system:
  - It is processed by executing a **chain of operators**.
  - These operators run over the **vector collection** to retrieve the results.

---

## Similarity Score

A similarity score f : RD × RD → R maps two Ddimensional
vectors, a and b, onto a scalar, f(a, b),
with larger values indicating greater similarity.

Here RD is Ddimensional vectors . 

Example 

<img src='assets\3d.png' alt='3d vector' >


Similarity Score is measured with the help of various distance algorithms .

-  Two vectors are considered similar if the distance between them is close to 0.

---

# Axioms of Distance Metrics

For a function to be considered a **valid distance metric**, it must satisfy the following properties:

### 1. Identity of Indiscernibles

- If the distance between two elements \( x \) and \( y \) is zero, then the two elements must be **identical**.
\[
d(x, y) = 0 \implies x = y
\]

### 2. Symmetry

- The distance between two elements should be the same regardless of their order.
\[
d(x, y) = d(y, x)
\]

### 3. Triangle Inequality

- For any three elements \( x, y, z \), the distance between \( x \) and \( z \) must be less than or equal to the sum of distances between the other two pairs.
\[
d(x, y) + d(y, z) \geq d(x, z)
\]

### 4. Non-Negativity

- Distances must always be **non-negative**.
\[
d(x, y) \geq 0
\]

---