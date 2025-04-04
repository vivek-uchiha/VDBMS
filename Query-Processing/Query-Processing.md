## Query Processing in a Vector Database Management System !

- Query processing in a **Vector Database Management System (VDBMS)** begins with a **search specification**.
- The search specification includes:
  - The **similarity score** (used to measure how close vectors are).
  - The **query type** (e.g.  nearest neighbor search).
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

**Triangular inequality** 

d(x,y)+d(y,z) >= d(x,z) - For any three elements x,y,z in the set, the sum of the distances between any two pairs must be greater than or equal to the distance between the third pair.

**Symmetry**

d(x,y)=d(y,x) - The distance between x and y should be same , irespective of the orders in which they are present

**Identity of indiscernibles**

- If the distance between two elements \( x \) and \( y \) is zero, then the two elements must be **identical**.  
- Mathematically:  
  \[
  d(x, y) = 0 \implies x = y
  \]
- This property ensures that the distance function distinguishes between different elements.



**Non-negativity**

d(x,y) >=0 The distance must be greater than 0.

---