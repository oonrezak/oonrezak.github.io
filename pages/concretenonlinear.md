## Formulating the Optimum Concrete Mix Using Machine Learning

<div class="gridwrapper">
  <div class="one"><img src="../images/concretenonlinear/correlations.png?raw=true"/></div>
  <div class="two"><img src="../images/concretenonlinear/benchmarks.png?raw=true"/></div>
  <div class="three"><img src="../images/concretenonlinear/mix_economy.jpg?raw=true"/></div>
  <div class="four"><img src="../images/concretenonlinear/feature_importances.png?raw=true"/></div>
</div>

<br />
### Keywords
* machine learning, regression, 
* benchmarking, optimization
* feature engineering
* feature importances, explainability

### Project Summary
Measuring concrete strength is difficult mainly because of the 28-day delay. As an example, I want to pour concrete for the 12th floor of my building. I do so, and also take some of the mix and mold it into cylinders. 28 days later, I find out that the concrete crushed at 30 MPa, when the design called for 40 MPa. I have several courses of action at this point, none of which are easy to implement. These choices include retrofitting at best, and in a worst-case scenario, demolishing the newly-built level and redoing the work.

Using data from the UCI ML Repository that contains information on the ingredients in concrete mixes as well as their tested compressive strengths, we want to predict the compressive strength of a new concrete mix based only from its ingredients.

Exploratory data analysis was done - pair plots were made and it was determined that among the ingredients of a concrete mix, cement has the greatest effect on concrete compressive strength. Different regression algorithms were benchmarked and the best algorithm was determine to be Gradient Boosting. Since GBM was already determined to provide the best accuracy, XGBoost was used and provided even better results than GBM. The highest accuracy obtained using XGBoost was 93.66% (averaged over 10 trials with different train-test splits).

In order to formulate the optimum concrete mix, the prices for each ingredient were be canvassed, and a brute-force iteration method was tried, where all possible concrete mixes were to be entered into the model, and the predicted strength of each taken. The optimum concrete mix is the formulation that yields a desired strength for a minimum price. However, this method failed due to the sheer number of possible permutations - iterating through them all would take several lifetimes. Thus, the data was revisited and the optimum concrete mix was taken from the samples.

To obtain a compressive strength of 40 MPa (this is the threshold of high-strength concrete), the optimum concrete mix was found to be:

* cement: 139.6kg
* slag: 209.4kg
* flyash: 0.0kg
* water: 192.0kg
* superplasticizer: 0.0kg
* coarseaggregate: 1047.0kg
* fineaggregate: 806.9kg

This mix should theoretically achieve a strength of 44.7 MPa, for a price of P2304.50 per cubic meter in 2019 (yields 19.40 KPa per PHP).

### Links
* [Notebook and Write-Up](/html_previews/concretenonlinear/concretenonlinear.html)
* [Project repository on github](https://github.com/oonrezak/concrete_nonlinear)
* [Back to Main Page](https://oonrezak.github.io/)