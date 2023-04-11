---
layout: page
title: Chance-constrained optimisation 
description: 
img: 
importance: 2
category: work
---


The scenario approach theory provides a beautiful mathematical property for the optimal solution of scenario programs (see optimisation problem below). It guarantees an upper bound on the probability of constraint violation of such optimal solution that can be used to generate, with high probability, a feasible solution to chance-constrainted optimization problems.
\\[\begin{align}
\mathrm{minimize} \quad  c^\top x \\
\quad \mathrm{subject~to} \quad  g(x,\delta) \leq 0, \forall \delta \in S. 
\end{align}\\]

I have contributed to the theoretical foundations of the scenario approach theory by showing the first tight bound for scenario programs with discarded constraints, a framework called the sampling-and-discarding scheme. I have recently explored the use of chance-constrained problems to generate feasible solutions to stochastic programming, combining this technique with the scenario approach theory to the design of stochastic barrier functions. Relevant papers are:

1. L. Romao, A. Papachristodoulou, K. Margellos, "On the exact feasibility of convex scenario programs with discarded constraints", IEEE Transaction on Automatic Control, 2023.
2. L. Romao, K. Margellos, A. Papachristodoulou, "Probabilistic feasibility guarantees for convex scenario programs with an arbitrary number of discarded constraints", Automatica, 2023.
3. F. Mathiesen, L. Romao, S. Calvert, A. Abate, L. Laurenti. "Inner approximations of stochastic programs for data-driven stochastic barrier function design", Technical report.
3. L. Romao, K. Margellos, A. Papachristodoulou, "Tight generalization guarantees for the sampling and discarding approach to scenario optimization", 59th Conference on Decision and Control (CDC), 2020.
4. L. Romao, K. Margellos, A. Papachristodoulou, "Tight sampling and discardind bounds for scenario programs with an arbitrary number of removed samples", L4DC, 2021.

