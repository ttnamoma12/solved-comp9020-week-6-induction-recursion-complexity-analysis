Download Link: https://assignmentchef.com/product/solved-comp9020-week-6-induction-recursion-complexity-analysis
<br>
<ol>

 <li>Prove by induction that 1 ⋅ 1! + 2 ⋅ 2! + … + n ⋅ n! = (n + 1)! − 1 for all n ≥ 1 (</li>

</ol>

n ∈ N).

<ol>

 <li>Given the definition,</li>

</ol>

s<sub>1 </sub>= 1

sn+1 = 1+1sn  (n &gt; 1)

prove by induction that FIB(n)

s<sub>n </sub>=

FIB(n + 1)

for all n ≥ 1 (n ∈ N).

<ol>

 <li>Suppose you would like to conclude that P(n) is true for all n ≥ 0 (n ∈ N). For each of the following conditions, determine whether the condition is sufficient to prove this.</li>

 <li>P(0) and ∀n ≥ 1(P(n − 1) ⇒ P(n + 1) ∧ P(n + 2)) ii. P(1) and ∀n ≥ 0(P(n + 1) ⇒ P(n) ∧ P(n + 2)) iii. P(0) and P(1) and ∀n ≥ 1(P(n) ∧ P(n + 1) ⇒ P(n + 2)) iv. P(0) and P(1) and ∀n ≥ 1(P(n) ⇒ P(n + 2))

  <ol>

   <li>P(0) and P(1) and ∀n ≥ 1(P(n) ⇒ P(2 ⋅ n) ∧ P(2 ⋅ n + 1))</li>

   <li>P(0) and P(1) and ∀n ≥ 1(P(2 ⋅ n) ⇒ P(2 ⋅ n − 1) ∧ P(2 ⋅ n + 1))</li>

  </ol></li>

</ol>

[show answer]

<ol start="2">

 <li>(Recursive definitions)</li>

</ol>

Recall the recursive definition of a rooted tree:

⟨v; ⟩                                  is a tree consisting only of a root node

⟨r;T<sub>1</sub>,T<sub>2</sub>,…,T<sub>k</sub>⟩⟩                          is a tree with root r and subtrees T<sub>1</sub>,T<sub>2</sub>,…,T<sub>k</sub> at the root (k ≥ 1)

Prove that in any rooted tree, the number of leaves is one more than the number of nodes with a right sibling.

<em>Hint:</em> This assumes a given order among the children of every node from left to right; see slide 22 (<a href="https://www.cse.unsw.edu.au/~cs9020/20T1/lecs/week7.pdf">week 7</a>) for an instance of this theorem.

[show answer]

<ol start="3">

 <li>(Recurrences)</li>

</ol>

Recall the recurrence for Mergesort:

T(1) = 0

T

Prove that n ⋅ (log<sub>2 </sub>n − 1) + 1 is a valid formula for T(n) for all n = 2<sup>k</sup> (with k ≥ 1).

[show answer]

<ol start="4">

 <li>(Asymptotic running times)

  <ol>

   <li>Suppose you have the choice between three algorithms:</li>

   <li>Algorithm A solves your problem by dividing it into five subproblems of half the size,</li>

  </ol></li>

</ol>

recursively solving each subproblem, and then combining the solutions in linear time. ii. Algorithm B solves problems of size n by recursively solving two subproblems of size n − 1 and then combining the solutions in constant time.

iii. Algorithm C solves problems of size n by dividing them into nine subproblems of size <u>n </u>, recursively solving each subproblem, and then combining the solutions in O(n2) 3 time.

Estimate the running times of each of these algorithms. Which one would you choose?

<ol>

 <li>Order the following functions in increasing asymptotic complexity:</li>

 <li>(n − 1) ⋅ (n − 2) ⋅ √n<sup>−</sup></li>

</ol>

3n ii.

<ul>

 <li>√−7−<sub>n</sub>−<sub>3</sub>−+−−3−<sub>n</sub>−+−−1</li>

</ul>

<ol>

 <li>5nlog(log(n))</li>

 <li>3nlog(n) + 2n<sup>2</sup></li>

 <li>8 + log(n) ⋅ (n − 1)</li>

</ol>

[show answer]

<ol start="5">

 <li>(Big-Oh)

  <ol>

   <li><em>Without using the Master Theorem,</em> give tight big-Oh upper bounds for the divide-andconquer recurrence T(1) = 1; T(n) = T( <u><sup>n</sup></u><sub>2 </sub>) + g(n), for n &gt; 1, where</li>

   <li>g(n) = 1 ii. g(n) = 2n iii. g(n) = n<sup>2</sup></li>

   <li>For each of the following functions, use the Master Theorem to determine the best upper bound complexity of T(n).</li>

   <li>T ii. T iii. T iv. T v. T

    <ol>

     <li>Analyse the complexity of the following recursive algorithm to test whether a number x occurs in an <em>unordered</em> list L = [x<sub>1</sub>,x<sub>2</sub>,…,x<sub>n</sub>] of size n. Take the cost to be the number of list element comparison operations.</li>

    </ol></li>

  </ol></li>

</ol>

<em>Search</em>(x,L = [x<sub>1</sub>,x<sub>2</sub>,…,x<sub>n</sub>]):

<strong>if</strong> x<sub>1 </sub>= x <strong>then return</strong> yes

<strong>else if</strong> n &gt; 1 <strong>then return</strong> <em>Search</em>(x,[x<sub>2</sub>,…,x<sub>n</sub>])

<strong>else return</strong> no

<ol>

 <li>Analyse the complexity of the following recursive algorithm to test whether a number x occurs in an <em>ordered</em> list L = [x<sub>1</sub>,x<sub>2</sub>,…,x<sub>n</sub>] of size n. Take the cost to be the number of list element comparison operations.</li>

</ol>

<em>BinarySearch</em>(x,L = [x<sub>1</sub>,x<sub>2</sub>,…,x<sub>n</sub>]):

<strong>if</strong> n = 0 <strong>then return</strong> no

<strong>else if</strong> <sup>x</sup><sub>⌈</sub><u>n</u>⌉ &gt; x <strong>then return</strong> <em>BinarySearch</em>(x,[x<sub>1</sub>,…,<sup>x</sup><sub>⌈</sub><u>n</u>⌉−1])

2                                                                                                                                                                               2

<strong>else if</strong> <sup>x</sup><sub>⌈</sub><u>n</u>⌉ &lt; x <strong>then return</strong> <em>BinarySearch</em>(x,[<sup>x</sup><sub>⌈</sub><u>n</u>⌉+1,…,x<sub>n</sub>])

2                                                                                                                                                 2

<strong>else return</strong> yes

[show answer]

<h1>6.  Challenge Exercise</h1>

Prove by induction that every connected graph G = (V,E) must satisfy e(G) ≥ v(G) − 1.

<em>Hint:</em> You can use the fact from a previous lecture that <sup>∑</sup><sub>v∈V </sub>deg(v) = 2 ⋅ e(G).

[show answer]