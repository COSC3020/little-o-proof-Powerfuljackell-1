# Little-o

"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice." 

Used prior approved work from: https://github.com/COSC3020/little-o-proof-Powerfuljackell

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$
adding the definition of big O for quick access
$T(n) \in O(f(n)) \iff \exists c>0, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$


Given that all constants must be great than 0 AND
Given that all n must be greater than $n_0$
Then based on the defition of $O$: $T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$
$f(n)\in o(g(n))$ implies that $f(n)\in O(g(n))$ because 
big O's requirements are less strict in that $f(n) \le c g(n)$ also contains $f(n) < c g(n)$
or anything that allows < to be true, also allows $\le$ to be true on top of the elements that it is equal too.
In addition c must exist in some form for big O, however in comparison little o's defenetion necessitates that c must work for any possible positive constant.
This further constrains little o to imply big O, as when c must fulfill all possible constants it also exists.
Thus, $f(n)\in o(g(n))$ implies that $f(n)\in O(g(n)) 
