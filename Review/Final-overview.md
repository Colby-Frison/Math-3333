# Comprehensive Exam Overview: Linear Algebra

In this class we used the textbook "Linear algebra and application by Kieth Nicholson", this exam will cover sections 3.1, 3.2, 3.3, 5.1, 5.2, 5.3, 5.4, 6.1, 6.2, 6.3, 7.1 and 7.2 from the textbook.

## 1. Vector Spaces (Sections 3.1, 3.2, 3.3)

### Fundamental Concepts
- **Definition of a vector space**: A set V with two operations (vector addition and scalar multiplication) satisfying 10 axioms
- **Subspaces**: A subset W of V that is itself a vector space under the operations of V
- **Span**: The set of all linear combinations of a set of vectors

### Axioms of Vector Spaces
1. **Closure under addition**: $u + v ∈ V$
2. **Commutativity of addition**: $u + v = v + u$
3. **Associativity of addition**: $(u + v) + w = u + (v + w)$
4. **Additive identity**: $∃0 ∈ V$ such that $u + 0 = u$
5. **Additive inverse**: $∀u ∈ V, ∃-u ∈ V$ such that $u + (-u) = 0$
6. **Closure under scalar multiplication**: $ku ∈ V$
7. **Distributivity of scalar over vector addition**: $k(u + v) = ku + kv$
8. **Distributivity of vector over scalar addition**: (k + m)u = ku + mu
9. **Associativity of scalar multiplication**: k(mu) = (km)u
10. **Scalar multiplication identity**: 1u = u

### Key Theorems
- **Subspace Test**: $W ⊆ V$ is a subspace iff:
  - $0 ∈ W$
  - $u, v ∈ W ⇒ u + v ∈ W$
  - $u ∈ W, k ∈ F ⇒ ku ∈ W$
- **Span is a subspace**: For any set $S ⊆ V, span(S)$ is a subspace of $V$

### Examples from Practice Problems
- Determining if a given set with unusual operations is a vector space (Problem 4, Set 5)
- Verifying vector space axioms (Problem 5, Set 5)
- Proving basic vector space properties (Problem 6, Set 5)
- Checking if subsets are subspaces (Problem 7, Set 5; Problem 1, Set 4)

## 2. Linear Independence, Basis, and Dimension (Sections 5.1, 5.2, 5.3, 5.4)

### Fundamental Concepts
- **Linear independence**: A set $\{v₁,...,vₙ\}$ is linearly independent if $c₁v₁ + ··· + cₙvₙ = 0 ⇒ c₁ = ··· = cₙ = 0$
- **Basis**: A linearly independent spanning set for $V$
- **Dimension**: The number of vectors in any basis for $V$
- **Coordinates**: The unique scalars when a vector is expressed as a linear combination of basis vectors

### Key Theorems
- **Replacement Theorem**: If V has a basis of n vectors, any linearly independent set in V has ≤ n vectors
- **Basis Extension Theorem**: Any linearly independent set can be extended to a basis
- **Dimension Theorem**: All bases for V have the same number of vectors
- **Rank-Nullity Theorem**: For linear transformation $T: V → W, dim(Null(T)) + dim(Range(T)) = dim(V)$
    - $dim(range(T)) = dim(codomain(T))$ = dimension of the output space
    - dim(V) = dimension of the input space
        - For polynomial spaces, the dimension is the degree of the polynomial plus 1
        - For $R^n$, the dimension is n
        - For $M_{m,n}$, the dimension is $m*n$

### Techniques
- Determining linear independence via row reduction
- Finding bases for subspaces
- Computing dimensions of subspaces
- Coordinate vector calculations

### Examples from Practice Problems
- Checking linear independence (Problem 6, Set 5; Problem 11, Set 4)
- Finding bases for subspaces (Problem 9, Set 5; Problem 7, Set 4)
- Dimension calculations (Problem 9, Set 5)
- Proving linear independence (Problem 11, Set 4)

## 3. Linear Transformations (Sections 6.1, 6.2, 6.3)

### Fundamental Concepts
- **Linear transformation**: A function $T: V → W$ satisfying:
  - $T(u + v) = T(u) + T(v)$
  - $T(ku) = kT(u)$
- **Kernel (Null space)**: $Null(T) = {v ∈ V | T(v) = 0}$
- **Range (Image)**: Im(T) = {T(v) | v ∈ V}
- **Rank**: dim(Im(T))
- **Nullity**: dim(Null(T))

### Key Theorems
- **Rank-Nullity Theorem**: For $T: V → W, dim(V) = rank(T) + nullity(T)$
    - explained more in depth earlier in the document
- **Matrix Representation**: Every linear transformation between finite-dimensional spaces can be represented by a matrix
- **Composition of Transformations**: $(S∘T)(v) = S(T(v))$ is linear if $S$ and $T$ are linear

### Techniques
- Verifying if a function is linear
- Finding bases for null space and range
- Determining if a transformation is one-to-one or onto
- Computing matrix representations

### Examples from Practice Problems
- Computing null space bases (Problem 1, Set 6)
- Determining if transformations are one-to-one/onto (Problem 1, Set 6)
- Finding matrix representations (Problem 4, Set 3)
- Composition of transformations (Problem 4, Set 3)

## 4. Determinants (Sections 7.1, 7.2)

### Fundamental Concepts
- **Determinant**: A scalar value associated with a square matrix
- **Cofactor expansion**: Method for computing determinants using minors and cofactors
- **Adjoint matrix**: Transpose of the cofactor matrix

### Properties of Determinants
1. $det(I) = 1$
2. $det(Aᵀ) = det(A)$
3. $det(AB) = det(A)det(B)$
4. $det(A^{-1}) = \dfrac{1}{det(A)}$
5. $det(kA) = kⁿdet(A)$ for n×n matrix A
6. If A has a row/column of zeros, $det(A) = 0$
7. If A has two identical rows/columns, $det(A) = 0$
8. Row operations:
   - Swapping rows: det changes sign
   - Scaling a row by k: det scales by k
   - Adding a multiple of one row to another: det unchanged

### Key Theorems
- **Cramer's Rule**: Solution to $Ax = b$ when $A$ is invertible
- **Invertibility Criterion**: $A$ is invertible ⇔ $det(A) ≠ 0$
- **Product Rule**: $det(AB) = det(A)det(B)$

### Techniques
- Computing determinants via cofactor expansion
- Using row operations to simplify determinant calculations
- Applying determinant properties to solve problems
- Finding inverses using adjugate matrices

### Examples from Practice Problems
- Computing determinants (Problem 1, Set 3)
- Cofactor expansions (Problem 1, Set 3)
- Determinant properties (Problem 2, Set 3)
- Special cases (Problem 3, Set 3)
- Determinant calculations with variables (Problem 8, Set 3)

## 5. Eigenvalues and Eigenvectors (From Practice Problems)

### Fundamental Concepts
- **Eigenvalue**: A scalar $λ$ such that $Av = λv$ for some $v ≠ 0$
- **Eigenvector**: A nonzero vector v satisfying $Av = λv$
- **Characteristic polynomial**: $p(λ) = det(A - λI)$
- **Eigenspace**: The null space of $A - λI$

### Key Theorems
- **Diagonalization**: $A$ is diagonalizable if it has n linearly independent eigenvectors
- **Similarity**: $A$ and $B$ are similar if $B = P⁻¹AP$
- **Cayley-Hamilton Theorem**: $p(A) = 0$ where $p$ is the characteristic polynomial

### Techniques
- Finding eigenvalues via characteristic polynomial
- Computing eigenvectors by solving (A - λI)v = 0
- Diagonalizing matrices when possible
- Computing powers of matrices using diagonalization

### Examples from Practice Problems
- Finding eigenvalues/eigenvectors (Problem 4, Set 3; Problem 9, Set 3)
- Geometric interpretations (Problem 4, Set 3)
- Diagonalization (Problem 10, Set 3; Problem 11, Set 3)
- Matrix powers via diagonalization (Problem 11, Set 3)

## 6. Matrix Algebra and Applications

### Fundamental Concepts
- Matrix operations: addition, multiplication, scalar multiplication
- Special matrices: symmetric, skew-symmetric, upper/lower triangular
- Matrix inverses and properties
- Elementary matrices and row operations

### Key Theorems
- Invertible Matrix Theorem (multiple equivalent conditions)
- Properties of matrix operations (associativity, distributivity)
- Relationship between elementary matrices and row operations

### Techniques
- Matrix multiplication and inversion
- Solving systems using matrix methods
- Using elementary matrices to understand row operations

### Examples from Practice Problems
- Matrix operations (Problem 4, Set 3)
- Elementary matrices (Problem 5, Set 3)
- Special matrices (Problem 7, Set 5; Problem 9, Set 5)

## 7. Problem-Solving Strategies

1. **Subspace verification**: Check closure under addition and scalar multiplication
2. **Basis finding**: Use row reduction to identify linearly independent vectors
3. **Linear independence**: Set up $c₁v₁ + ··· + cₙvₙ = 0$ and solve
4. **Determinant calculation**: Use cofactor expansion or row operations
5. **Eigenvalue problems**: Solve $det(A - λI) = 0$, then find null space of $A - λI$
6. **Diagonalization**: Find P (eigenvectors) and D (eigenvalues)
7. **Linear transformations**: Verify properties or find matrix representations

## 8. Important Proof Techniques

1. **Subspace proofs**: Verify the three conditions (contains 0, closed under + and scalar multiplication)
2. **Linear independence proofs**: Assume a linear combination equals 0 and show all coefficients must be 0
3. **Basis proofs**: Show linear independence and spanning
4. **Transformation linearity**: Verify $T(u+v) = T(u)+T(v)$ and $T(ku) = kT(u)$
5. **Determinant properties**: Use row operations and expansion theorems
6. **Eigenvalue arguments**: Work directly from the definition Av = λv

## 9. Common Problem Types to Expect

Based on the practice sets, expect problems involving:
- Verifying vector space axioms
- Determining if subsets are subspaces
- Finding bases for subspaces
- Checking linear independence
- Computing determinants
- Finding eigenvalues/eigenvectors
- Diagonalizing matrices
- Analyzing linear transformations (kernel, range, one-to-one, onto)
- Solving systems of equations
- Working with special matrices (symmetric, skew-symmetric, etc.)
- Proving basic linear algebra theorems
- Applications of the Rank-Nullity Theorem
- Properties of determinants and their applications

## 10. Key Formulas to Remember

1. **Determinant of 2×2 matrix**: $\det\left(\begin{bmatrix} a & b \\ c & d \end{bmatrix}\right) = ad - bc$
2. **Cofactor expansion**: $det(A) = Σ(-1)^{(i+j)}a_{ij}M_{ij}$ for any row i or column j
3. **Characteristic polynomial**: det(A - λI) = 0
4. **Rank-Nullity**: dim(V) = rank(T) + nullity(T)
5. **Inverse via adjugate**: $A^{-1} = \frac{1}{\det(A)} \operatorname{adj}(A)$
6. **Diagonalization**: $A = PDP⁻¹ ⇒ Aⁿ = PD^nP^{-1}$
7. **Eigenvalue sum**: $Σλ_i = trace(A)$
8. **Eigenvalue product**: $Πλ_i = det(A)$
