# Lisp
simple lisp programs

Given a set of numbers N={x1, x2,.., xn} and a capacity C, the subset sum problem is the problem of finding a subset of N, S N, such that the sum of the numbers in S is maximal and is less than or equal to C.
Example: If C=10 and N={2,3,11,6}, the maximal subset sum is 3+6=9 
(Note that the subset-sum problem is a special case of the famous 0-1 knapsack problem where item weights are the same as item values. 

1)Write a program named “subset-sum1” that returns the maximal subset sum. (subset-sum1 numbers capacity) The name of the top-level function should be “subset-sum1”. The first parameter “numbers” is a list of integers, and the second parameter “capacity” represents the capacity. Example: (subset-sum1 ’(1 2 18 2 2) 20) => 20 

2)Write an extended version of the program you wrote for (1) above which returns both the maximal subset sum as well as the list of integers that are selected to be included. Example: (subset-sum2 ’(1 2 18 2 2) 20) => (20 ’(2 18)) You are allowed to use only the following primitives:  ￼ numbers, symbols, variables t , nil defun, let, quote, ', arithmetic/comparison operators 演算,比較: +, -, /, * , =, <=, >=, <, >, boolean operators 論理演算: and or not List manipulation リスト構造の操作: first rest car cdr cons list append, null, atom conditional forms 条件: if, cond,
