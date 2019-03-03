#  Superconductor Critical Temperature Predictions
 
 
 
## Contents of Repository 
 
[Superconductor_statistics.ipynb](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_statistics.ipynb):
 
[Superconductor_clustering.ipynb](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_clustering.ipynb):
 
[Superconductor_linear_reg.ipynb](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_linear_reg.ipynb):
 
[Superconductor_gradient_boosting.ipynb](https://github.com/fullmetalchem15t/superconductors/blob/master/Superconductor_gradient_boosting.ipynb):
 
## Purpose
 
In this project, the critical temperature of superconductors is modeled and predicted. This is based on the work of Ken Hamidieh <https://arxiv.org/abs/1803.10260>. We are adding clustering based the observation that the data is bimodal. We will determine if clustering improves prediction.
 
## Method
 
There are three part to this project, clustering, linear regression, and gradient boosting. The data was clustered into two groups based on the observation that the data is bimodal. Before performing linear regressions or gradient boosting, the data was standardized (attribute values set to z score). For both linear regression and gradient boosting, the data was modeled separated by cluster. An additional model of each method was made for the uncluster data.
## Results

* For the linear regression model:
  - The RMSE for the Unclustered model was 19.50 K
  - The RMSE when clustering was 17.36 K
  - Clustering did improve accuracy of linear regression model
 
* For the gradient boosting model:
  - The RMSE for the Unclustered model was 11.40 K
  - The RMSE when clustering was 11.56 K
  - Clustering did not improve accuracy of gradient boosting model 

## Conclusion

Will come soon.
