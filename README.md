# Product of Array Except Self

## Problem Statement

Given an integer array `nums`, return an array `answer` such that:

`answer[i]` is equal to the product of all elements of `nums` except `nums[i]`.

The solution should be implemented without using division.

## Example

### Input
[1, 2, 3, 4]

### Output
[24, 12, 8, 6]

## Explanation

For each element:

- 1 → 2 × 3 × 4 = 24
- 2 → 1 × 3 × 4 = 12
- 3 → 1 × 2 × 4 = 8
- 4 → 1 × 2 × 3 = 6

Therefore, the output is:

[24, 12, 8, 6]

## Approach

The solution uses two passes:

1. Store the product of all elements to the left of each index.
2. Traverse from right to left and multiply by the product of all elements to the right.

This avoids using division.

## Complexity

- Time Complexity: O(n)
- Space Complexity: O(1) extra space

## Language

Java

## Author

M. Pallavi
