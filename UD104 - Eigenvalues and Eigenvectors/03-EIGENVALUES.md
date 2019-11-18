# EIGENVALUES

In machine learning,the ability to transform a vector by a scalar factor is very useful.

Matrices that have the ability to scale a vector are called Eigenvectors and the scaling factor is called an Eigenvalue.

An Eigenvector is a vector that when multiplied by a given transformation matrix is a scalar multiple (Eigenvalue) of itself.

```
Given the transformation matrix:

[3 -2]
[1  0]

[2]
[1]

is an Eigenvector for the given matrix.

Because the linear transformation results in,

[4]
[2]

which is a scalar multiple of itself by 2. Hence the Eigenvalue is 2.
```

### Calculating Eigenvalues

Lets define:

- A as the transformation matrix
- X as the Eigenvector
- λ as the Eigenvalue

When we say that the vector only changes in magnitude and not the direction, the following must be true:

```
A.X = λ.X
```

We introduce an identity matrix (denoted by I) into the equation. The identity matrix (or the unit matrix) is a square matrix of size n \* n with ones on the main diagonal and zeroes in other positions. When you multiply the transformation matrix with the identity matrix, we get the same transformation matrix.

```
[3 -2]  *  [1 0]  =  [3 -2]
[1  0]     [0 1]     [1  0]
```

```
Hence our equation becomes,

A.X = λ.I.X

This can be simplified to,

(A - λ.I).X = 0
```

We need to find the non-trivial or non-zero solution for this equation.

If (A - λ.I) is invertible (determinant is non-zero), then it can be divided on both sides and we end up with X = 0.

So, we need to find λ, such that A - λ.I is not invertible, that is, the determinant of A - λ.I needs to be 0.

```
det(A - λ.I) = 0

This is known as the characteristic equation.
```

```
A - λ.I = 0

=>

[3 -2] - [λ 0] = [3 - λ   0]
[1  0]   [0 λ]   [0      -λ]
```

The determinant of the matrix is,

```
-3.λ + λ^2 - 0 = 0
```

which resolves to,

```
λ.(λ - 3) = 0
```

Therefore, λ = 3 (or) 0.

Similarly if, A is

```
[2  3]
[3 -6]
```

Then,

```
[2  3] - [λ 0] = [2-λ    3]
[3 -6]   [0 λ]   [3   -6-λ]


(2-λ)*(-6-λ) - 3.3 = 0

-12-2λ+6λ+λ^2 - 9 => λ^2 + 4λ - 21 = 0

(λ + 7) * (λ - 3) = 0
λ = 3 (or) -7
```
