#  Superconductor Critical Temperature Predictions
 
 
 
## Contents of Repository 
 

[Superconductor_statistics.ipynb](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_statistics.ipynb):
Data initialization and statistics overview.
 
[Superconductor_clustering.ipynb](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_clustering.ipynb):
 Clustering notebook

[Superconductor_linear_reg.ipynb](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_linear_reg.ipynb):
 Linear regression notebook

[Superconductor_gradient_boosting.ipynb](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_gradient_boosting.ipynb): Gradient boosting notebook.

[Superconductor_Slides.pdf](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_Slides.pdf) : In progress
 
## Purpose
 
In this project, the critical temperature of superconductors is modeled and predicted. This is based on the work of 
[Ken Hamidieh](https://arxiv.org/abs/1803.1026). We are adding clustering based the observation that the data is bimodal. We will determine if clustering improves prediction.
 
## Method
 
There are three part to this project, clustering, linear regression, and gradient boosting. The data was clustered into two groups based on the observation that the data is bimodal. Before performing linear regressions or gradient boosting, the data was standardized (attribute values set to z score). For both linear regression and gradient boosting, the data was modeled separated by cluster. An additional model of each method was made for the uncluster data.
## Results

* For the linear regression model:
  - The Unclustered model has an RMSE 19.50 K and an r$^2$ of 0.70.
  - When clustering the RMSE is 17.36 K and the r$^2$ is 0.76.
  - Clustering did improve accuracy of linear regression model.
 
* For the gradient boosting model:
  - The RMSE for the Unclustered model was 11.40 K and an r$^2$ of 0.90. 
  - When clustering, the RMSE is 11.56 K and the r$^2$ is 0.89.  
  - Clustering did not improve accuracy of gradient boosting model.

## Conclusion

The critical temperature of superconductors were predicted with a high level of accuracy. As suspected, gradient boosting performed better than linear regressions. Clustering had improved the results of the linear regression model but little effect on gradient boosting model. Clustering may have improved results for linear regression accuracy if the relationship between the properties and critical temperature is non-linear. Clustering fragmented the prediction into two different linear fits regions which was more flexible than a single linear fit. The gradient boosting method is nonlinear and as a flexible enough that it does not need different models for feature value regions.

 
While not examined here as of yet, it would be interesting to determine how well a predictive model can do using the elements in the superconductors alone. The feature properties were derived from elemental components alone, not the superconductor. The properties may be a proxy for the elemental components.

