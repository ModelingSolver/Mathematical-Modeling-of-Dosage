# Mathematical-Modeling-of-Dosage

*The Path to Mathematical Resolution of a Non-Linear Algorithm (Dosage Problem)*

We start with a pancake recipe, or "pancake algo"... We consider the "dosage" sub-algo..

_Problem:_ We have a dosage algorithm that takes the size of an egg (T) as input and outputs the quantity of flour (F) and milk (L) needed to make pancakes.
- Three egg sizes here, T1, T2, and T3.
- If small egg, 100g flour,
- If medium egg, 130g flour,
- If large egg, 150g flour
- If 100g F, 200ml milk
- If 130g F, 260ml milk
- If 150g F, 300ml milk

_Data:_
- Piecewise equations
- F(T) = { 100 if T = T1, 130 if T = T2, 150 if T = T3 }
- L(T) = { 200 if T = T1, 260 if T = T2, 300 if T = T3 }

1. _Definition of Basic Equations:_
- F(T) = { 100 if T = T1, 130 if T = T2, 150 if T = T3 }
- L(T) = { 200 if T = T1, 260 if T = T2, 300 if T = T3 } (Non-solvable system!!)

2. _Mathematical Representation:_
Kronecker notation
- F(T) = Σ (F_i * δ(T-T_i)) for i = 1 to 3
- L(T) = Σ (L_i * δ(T-T_i)) for i = 1 to 3

3. _Searching for a Link..._
Discovery of the link between F(T) and L(T):
- F(T_i) / L(T_i) = 0.5 for all T_i
- L(T) = 2 * F(T)

4. _YES AND LOL System Resolution:_
- F(T) = { 100 if T = T1, 130 if T = T2, 150 if T = T3 }
- L(T) = 2 * F(T) = { 200 if T = T1, 260 if T = T2, 300 if T = T3 }
- And voilà! We have solved the system by discovering the link between F(T) and L(T), which allows us to calculate the quantity of milk needed based on the quantity of flour.
- USELESSLY PAWAFOOL :smirk:
