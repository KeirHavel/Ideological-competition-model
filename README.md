# Ideological-competition-model

# Summary

A model of two competing ideologies that occaisonally become violent. Slightly based on the excercise 8.1.15 in Strogatz' Nonlinear Dynamics and Chaos. There are two ideologies in population undergoing logistic growth, A and B (there are also neutral people with no ideology); both ideologies start at the same frequency (1/4 of people) in the population. Both have an intrinsic rate of violence. To determine how likely an ideology is to become violent, it's intrinsic rate of violence is tested against a randomly generated number (which is the same for both ideologies, hence they become violent at similar times). If it is greater than the number, the ideology will become violent, otherwise it will not. This model tests how likely an ideology is to become ubiqitous in a population given its rate of violence and a factor called repulsiveness, which measures how repulsed people are by an ideology's violence. The notebook file has more in-depth information as it is being implemented.

# Results


The image that follows depicts the results of the model.


![result image](https://raw.githubusercontent.com/KeirHavel/Ideological-competition-model/master/idea_comp.png)

A blue pixel means one ideology (B) achieved complete dominance in a population after 1000 years, red means the other ideology (A) succeeded (purple indicated coexistence). The y-axis depicts the violence of the ideology. At y=0 ideology B (blue) has maximal violence and ideology A is non-violent. On the other end, at y=1 (pixel 1080) ideology A (red) has maximal violence and B is pacifistic (hence the symmetry around the central horizontal axis, which shows that the model's outputs were statistically similar for each ideology). A black pixel indicates extinction, i.e. both ideologies killed each other.

At x=0, the "repulsiveness" is 2. That means that violent ideologies lose followers at twice the rate as non-violent ideologies. At the other extreme (x=5, pixel 1920), violent ideologies lose followers at six times the rate as nonviolent ideologies. As can be seen, greater repulsiveness prevents one ideology from beating another and becoming dominant. The band structure (especially the increased extinction rate around x=3.5 (center-right of image) is difficult to explain. It could be a strange bug, but may also be an intrinsic feature of the model.
