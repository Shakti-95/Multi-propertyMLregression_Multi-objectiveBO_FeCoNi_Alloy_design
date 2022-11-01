#Accelerated Design of Multi-property FeCoNi alloy using Machine Learning and Bayesian Optimization

This work under final stage of preparation for manuscript submission.

* Historically, material development and deployment is a long and expensive process. Starting from development of a new material from lab to meeting the industrial criterias to finally commercially deploying the material in a particular application, it takes nearly 20 years and millions of dollars is spent. In material development, mainly 3 types of methodologies are followed - trial and error experiments, theoretical laws and modelling, and high performance computer based simulations. However, with the advent of data-driven science, the use of machine learning in materials development is a boon in terms of reducing time and cost and increasing efficient search. 

* One such class of materials are magnetic alloys and commercially there is no alloy with optimized multi-property. FeCoNi is a potential alloy which can offer high saturation magnetization due to presence of Fe and Co, low coercivity due to presence of Ni, high Curie temperature due to presnce of Co, high mechanical strength due to Co and Ni, and moderate electrical resistivity due to presence of Ni.

* Therefore, in this work, a database of previous experimental research was curated and analyzed. The total number of data entries are 1208. Upon analysis, it was observed that multi-property study was very less performed in the past and hence there were gaps in property data. 

* An unique ML based imputation technique was developed in which 12 types of regressors were built (machine learning and deep learning) and the best model was chosed based on lowest MAE to fill up each property. 

* Later, this imputed database was used to develop multi-input multi-output regression models (Random Forest, Extra Trees, and 2 types of Deep Neural Network architectures) and the best model with lowest MAEs for all the properties was chosen. The chosen multi-property model was then experimentally validated using 40 FeCoNi compositions synthesized and characterized by high-throughput methodology.

* Further, a multi-objective Bayesian optimization was developed to design FeCoNi alloy compositions. In this, target values for saturation magnetization, Curie temperature, and cost of raw material are set and the objective function was defined in such a way that gaussian process regressor finds the composition such that the absolute difference between the predicted and target property values is minimum.

* Finally, the predicted compositions and their predicted property values were experimentally validated. 2 novel FeCoNi alloy compositions are developed.

The codes for each step will be available shortly!
