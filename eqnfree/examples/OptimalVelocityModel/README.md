# Example: Optimal velocity model
In this directory, an example code is given for the computation of a bifurcation analysis of an optimal  velocity model. It uses the OVM code from my repository "optimal_velocity_model". In this model, cars are driving on a circuit. Depending on the specific parameter settings traffic jams appear/are not present. The occurence of a jam can be measured (for instance) by the standard deviation of the headways (distance to the leading car). If the standard deviation of the headways is 0, no traffic jam is present. If it is non-zero a jam wave is present in the model.

In specific, this code computes and plots the bifurcation diagram as done in Marschler et al. (2014). The bifurcation analyses is done for the parameter "v0" that is the velocity scale of the model and the standard deviation of the headways as measure for the traffic jam. Currently, the bifurcation diagram computed by this code is not 100% equal to Marschler et al. (2014). This problem would be even smaller if new reference states would be computed during the analysis. Right now it is circumvented by having a larger "tskip" and "delta" value than in Marschler et al. (2014).

## Literature
Marschler, C., Sieber, J., Berkemer, R., Kawamoto, A., & Starke, J. (2014). Implicit methods for equation-free analysis: convergence results and analysis of emergent waves in microscopic traffic models. SIAM Journal on Applied Dynamical Systems, 13(3), 1202-1238.