# Mars Spectrometry: Detect Evidence for Past Habitability Competition

<img src="assets/nasa-mars-curiosity.jpg" alt="pipeline/nasa-mars-curiosity" />

*Image courtesy of
[NASA/JPL-Caltech/MSSS.](https://mars.nasa.gov/resources/26384/two-versions-of-a-curiosity-selfie-narrow-and-wide/)*

## General
* **Problem statement:** Build a model to automatically analyze mass spectrometry data collected for Mars exploration in order to help scientists in their analysis of understanding the past habitability of Mars.
* **Type:** Multi-Label Classification
* **Host:** NASA
* **Platform:** Drivendata
* **Competition link:** https://www.drivendata.org/competitions/93/nasa-mars-spectrometry/
* **Placement:** Top 3% (23/713)

## Lessons learned
* Differences between XGBoost, LightGBM and CatBoost
* Tree methods don´t care about outliers
* Decision-Tree based models still beat deep learning models, when working with tabular data
* How to use Optuna for hyperparameter search
* A solution can be worked out within a small windows (1 week)
* Binary relevence method to solve multi-label classification problems (similar to OvA & OvR)
* XGBoost, LightGBM and CatBoost are non-deterministic. You have to do multiple hypermeter searches to find best parameters

## Future approaches
* Try out different approaches to solve multi-label classification
* Use weighted ensembles for each label. Weight depends on performance of classifier
* Try out under-/oversampling
* More details on model performance to spot underfitting/overfitting
