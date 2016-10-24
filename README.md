# pgxsimulation

The `pgxsimulation` tool will be used for the simulation of one genetic variant for data from a randomized clinical trial. Genetics (**`G`**), treatment arm (**`T`**) and events (**`E`**) will be simulated using a logistic regression model of **`GxE`** interaction. Parameters defined by the user required to conduct the simulation include: minor allele frequency, baseline event risk, treatment odds ratio and genetics odds ratio in both the placebo and the treatment arm.

Four statistical models will be compared for statistical power and error rate. The first model consists of a logistic regression (**`E ~ G`**) using only the treatment arm. The second model is an interaction model (**`E ~ G + T + GxT`**) using the complete simulated cohort. The third model is a case only analysis (**`T ~ G`**). The fourth model is a stratified analysis by genotype categories (**`E ~ T`** for each of the three possible genotypes).

The `pgxsimulation` tool will provide a web interface to launch the simulations and show results to the user.
