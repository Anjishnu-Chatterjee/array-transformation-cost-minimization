# Array Transformation Cost Minimization

Java solution for Problem 2: Array Transformation Cost Minimization.

## Problem

Given an integer array `A` of size `N`, you can replace any `A[i]` with either:

- `A[i] + K`
- `A[i] - K`

Find the minimum total number of operations needed to make all array elements equal. If it is impossible, print `-1`.

## Approach

All elements can become equal only if they have the same remainder when divided by `K`.

After that, divide the values by `K`. The best target value is the median, because the median minimizes the sum of absolute differences.

## Example

```text
Input:
5
2 4 6 8 10
2

Output:
6
```

## Run

```powershell
javac Main.java
@"
5
2 4 6 8 10
2
"@ | java Main
```

## Complexity

- Time complexity: `O(N log N)`
- Space complexity: `O(N)`
