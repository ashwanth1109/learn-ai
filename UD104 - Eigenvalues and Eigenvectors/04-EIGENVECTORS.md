# EIGENVECTORS

We have simplified our equation before to,

```
(A-λ.I).X = 0

Our transformation matrix A is,
[5  6]
[3 -2]

We calculated the eigenvalues to our equation to be,

λ1 = 7
λ2 = -4
```

If we substitute the value 7,

```
[5  6] - [7  0] = [-2  6]
[3 -2]   [0  7]   [3  -9]
```

We define our eigenvector as X1 and X2,

```
[-2  6] * [X1] =>
[3  -9]   [X2]

Solving this for 0, we get the linear equations,
-2X1 + 6X2 = 0
3X1 - 9X2 = 0

Equating the two,
X1 - 3X2 = 0
```

This equation has many non-zero solutions (but dependant)

```
Examples:
[3]  (or)  [9]  (or)   [-6]
[1]        [3]         [-2]
```

We can pick one solution as the vector we are looking for.
