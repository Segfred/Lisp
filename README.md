# Lisp
Given a set of numbers N={x1, x2,.., xn} and a capacity C,
the subset sum problem is the problem of finding a subset of N, S N, such that the sum of the numbers in S is maximal and is less than or equal to C.
Example: If C=10 and N={2,3,11,6}, the maximal subset sum is 3+6=9
容量 C と n 個の整数の集合 N={x1, x2,.., xn}を与えられた場合、
N の部分集合 S, S N のうち、部分集合に含まれる数の総和(但し総和は容量 C 以下)を 最大化する部分集合を求める問題を部分和問題と呼ぶ。
例: 容量が C=10 の場合、N={2,3,11,6}の最大部分和は 9 ( 3+6)
(Note that the subset-sum problem is a special case of the famous 0-1 knapsack problem where item weights are the same as item values. 部分和問題はアイテムの価値と重みが 等しい特殊な 0-1 ナップサック問題である。)
1)Write a program named “subset-sum1” that returns the maximal subset sum. 部分和問題の最大部分和を返す、プログラムを書きなさい。
(subset-sum1 numbers capacity)
The name of the top-level function should be “subset-sum1”. The first parameter “numbers” is a list of integers, and the second parameter “capacity” represents the capacity.
関数の名前は subset-sum1, 1番目の引数は numbers は整数のリスト、2番麺の引数 capacity は容量。
Example: (subset-sum1 ’(1 2 18 2 2) 20) => 20
2)Write an extended version of the program you wrote for (1) above which returns both the maximal subset sum as well as the list of integers that are selected to be included. (1)のプログラムを、最大部分和だけでなく、最大和部分集合も返すプログラムを 書きなさい
(subset-sum2 numbers capacity)
Example: (subset-sum2 ’(1 2 18 2 2) 20) => (20 ’(2 18))
You are allowed to use only the following primitives:
以下の関数等を使用してよい。
￼
numbers, symbols, variables
t , nil
defun, let, quote, ',
arithmetic/comparison operators 演算,比較: +, -, /, * , =, <=, >=, <, >, boolean operators 論理演算: and or not
List manipulation リスト構造の操作: first rest car cdr cons list append, null, atom conditional forms 条件: if, cond,
