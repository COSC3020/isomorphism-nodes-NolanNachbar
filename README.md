# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Given two graphs, $G_1=(V_1 , E_1)$ and $G_2 = (V_2, E_2)$. Consider the case where $|V_1| \neq |V_2|$, this means that either  $|V_1| > |V_2|$ or $|V_1| < |V_2|$. 
Now suppose there's a function  $f: V_1 \rightarrow V_2$ such that $(u,v) \in E_1$ iff $(f(u),f(v)) \in E_2$. The cardinalities must fall into one of two cases.

- Case 1: $|V_1| > |V_2|$
   By the pigeon hole theorem, $(u,v) \in E_1$ iff $(f(u),f(v)) \in E_2$ would mean that there is at least one instance where $2$ or more different vertices in $G_1$ would be mapped to a single vertex in $G_2$. Thus the mapping isn't injective (one-to-one), and the graphs can't be isomorphic.

- Case 2: $|V_1| < |V_2|$
   There are more vertices in $G_2$ than in $G_1$ so there must be one or more veritces in $G_2$ that have no mapping from $G_1$. Thus $f$ isn't surjective (onto), and the graphs are not isomorphic.

  Thus in both cases, if two graphs $A$ and $B$ do not have the same number of nodes, they cannot be isomorphic.

I certify that I have listed all sources used to complete this exercise, including the use of any large language models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice. 

I did this all independently except for reveiwing bijective functions with this:
https://www.geeksforgeeks.org/bijective-function/#
