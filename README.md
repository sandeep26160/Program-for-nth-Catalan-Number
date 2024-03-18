# Program-for-nth-Catalan-Number
Catalan numbers are defined as a mathematical sequence that consists of positive integers, which can be used to find the number of possibilities of various combinations. 

The nth term in the sequence denoted Cn, is found in the following formula: 

*** QuickLaTeX cannot compile formula:
\frac{(2n)!}{((n + 1)! n!)}       

Catalan numbers occur in many interesting counting problems like the following.

Count the number of expressions containing n pairs of parentheses that are correctly matched. For n = 3, possible expressions are ((())), ()(()), ()()(), (())(), (()()).
Count the number of possible Binary Search Trees with n keys (See this)
Count the number of full binary trees (A rooted binary tree is full if every vertex has either two children or no children) with n+1 leaves.
Given a number n, return the number of ways you can draw n chords in a circle with 2 x n points such that no 2 chords intersect.

Examples:

Input: n = 6
Output: 132

Input: n = 8
Output: 1430

Step-by-step approach:

Base condition for the recursive approach, when n <= 1, return 1
Iterate from i = 0 to i < n
Make a recursive call catalan(i) and catalan(n – i – 1) and keep adding the product of both into res.
Return the res.
