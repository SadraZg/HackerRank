Johnny is playing with a large binary number, B. The number is so large that it needs to be compressed into an array of integers, A,
where the values in even indices (0, 2, 4, ...) represent some number of consecutive 1 bits and the values in odd indices (1, 3, 5, ...)
represent some number of consecutive 0 bits in alternating substrings of B.

For example, suppose we have array A={4, 1, 3, 2, 4}. A0 represents "1111", A1 represents "0", A2 represents "111", A3 represents "00",
and A4 represents "1111". 

When we assemble the sequential alternating sequences of 1's and 0's, we get B="11110111001111".

We define setCount(B) to be the number of 1's in a binary number, B. Johnny wants to find a binary number, D, that is the smallest 
binary number > B where setCount(B) = setCount(D). He then wants to compress D into an array of integers, C (in the same way that 
integer array A contains the compressed form of binary string B).

Johnny isn't sure how to solve the problem. Given array A, find integer array C and print its length on a new line. Then print the
elements of array C as a single line of space-separated integers.


Input Format

The first line contains a single positive integer, T, denoting the number of test cases. Each of the 2T subsequent lines describes 
a test case over 2 lines:
1. The first line contains a single positive integer, n, denoting the length of array A.
2. The second line contains n positive space-separated integers describing the respective elements in integer array A(i.e., A0, A1, ...).

Output Format
For each test case, print the following 2 lines:

1. Print the length of integer array C (the array representing the compressed form of binary integer D) on a new line.
2. Print each element of C as a single line of space-separated integers.
It is guaranteed that a solution exists.
