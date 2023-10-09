Maths Introduction

1. Working with the following set of Integers S = {0,1,2,3,4,5,6}

What is \
a) $4 + 4$ \ 
b) $3 * 5$ \ 
c) what is the inverse of 3 ? \

Answer: \
 a) $4 + 4 = 8 = 1 (\mod 7)$ \
 b) $3 * 5 = 15 = 1 (\mod 7)$ \
 c) From Fermat's Little Theorem
  $a ^ {-1} = a ^ {p-2} (\mod 7)$, so for $a = 3 $, it is \
$3 ^ {-1} = 3 ^ {7 - 2} = 3 ^ {5} = 5 (\mod 7)$.
  Also, we can verify the result from b) with this answer. \

2. For S = {0,1,2,3,4,5,6}, Can we consider 'S' and the operation '+' to be a group ? \

Answer: \
Assuming that '+' represent addition over modulo 7 we can, otherwise we cannot as we don't even have closure (for example, $3 + 6 = 9$ and $3, 6 \in S$ while $9 \notin S$). \

3. What is -13 mod 5? \
Answer: \
$-13 = -8 = -3 = 2 (\mod 5)$

4. Polynomials: \
 For the polynomial $x^3 − x^2 + 4x − 12$ \
 Find a the positive root? \
 What is the degree of this polynomial? \

Answer: \
One root is 2, (first tried out of candidates which divide 12). $2^3 - 2^2 + 4*2 - 12 = 8 - 4 + 8 - 12 = 0$
 If we try to divide given polynomial by (x - 2), we get $x^2 + x + 6$, which doesn't have solutions in real. Complex zeroes are $\frac{-1 \pm i \sqrt{23} }{2}$. \
 Degree of this polynomial is 3.
