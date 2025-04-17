# Vampire Case Study
The code repository for my Bachelor Thesis "Automated First-Order Theorem Proving" at Johannes Kepler Universität Linz.

All theorems use the same six axioms that hold for linear operators. They are commented in 02/input.txt.

For theorem 17, there are seperate input files for each equivalence between the 5 conditions. The files in the folder 'all_variables' have all variables in the forall statement that are needed by any of the 5 conditions. The files in 'necessary_variables' only have the variables that are needed by the 2 condition of the respective equivalence. For example, the variable 'ABC_' (representing ABC^deggar) is redundant for proving (2) <=> (3). Vampire could prove every equivalence when using all variables. Interestingly, when removing redundant variables, Vampire cannot find a proof for (2) <=> (5), (3) <=> (5), and (4) <=> (5) anymore.
