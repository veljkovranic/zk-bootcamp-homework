1. Modular arithmetic - you just need to find examples, you
don't need to prove anything. \

	1. Is it true that all odd squares are ≡ 1 (mod 8) ? \
	2. what about even squares (mod 8) ?\

Answer: \
 1. We get odd square $s$ by multiplying odd number with itself, otherwise it wouldn't be odd to begin with. Assuming that our odd number has a form of $2k+1$ and $s=(2k+1)(2k+1)=4k^2+4k+1=4k(k+1)+1$. Having $k \in Z$, either $k$ or $k+1$ will be even, and as such divisible by two, hence our $s$ can be written as $s=4*2*m+1$, where $m=\frac{k(k+1)}{2}$. \

 2. For even squares, we have $s=2k*2k=4k^2$, which for either parity of $k$ will give us either $1$ or $4$, as a result of $s \mod 8$.\

2. Try out the vanity bitcoin address example at asecurity
or the Ethereum version
	

3. What do you understand by
	1. O(n)
	2. O(1)
	3. O(log n)
For a proof size, which of these would you want ?

Answer: 
	2.