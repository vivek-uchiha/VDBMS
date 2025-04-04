## Query Processing in a Vector Database Management System !

- Query processing in a **Vector Database Management System (VDBMS)** begins with a **search specification**.
- The search specification includes:
  - The **similarity score** (used to measure how close vectors are).
  - The **query type** (e.g., nearest neighbor search).
- **Search criteria** are passed into the system via a **query interface**.
- Once the query is received by the system:
  - It is processed by executing a **chain of operators**.
  - These operators run over the **vector collection** to retrieve the results.


## Similarity Score

A similarity score f : RD × RD → R maps two Ddimensional
vectors, a and b, onto a scalar, f(a, b),
with larger values indicating greater similarity.

Here RD is Ddimensional vectors . 

Example 

!(3D Vector)[Query-Processing\assets\3d.png]