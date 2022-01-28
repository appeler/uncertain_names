uncertain names: uncertainty using dropout and conformal prediction
---------------------------------------------------------------------

Using the FL voter registration data and the base LSTM model, we illustrate how to produce uncertainty estimates using dropout and conformal prediction.

* [Dropout](notebooks/fl_ln_dropout.ipynb)
* [Conformal Prediction](notebooks/fl_ln_conformal.ipynb)

### Side-by-side

We randomly picked 10,000 `unseen` names (not in the training set) from the test set to illustrate how outputs differ across these cases. The output CSV has the following columns: last_name, label, conformal_pred_set, lw_ci_nh_white, up_ci_nh_white, ...

Here's a short snippet of the output:


### Application

We compare the average CI and the average size of the prediction set (via conformal inference) of `seen` names to `unseen` names as one of the applications of uncertainty estimates. As the following [notebook](notebook/compare_seen_unseen.ipynb) illustrates, the average set size and average CI is slightly smaller for `seen` names.

### Authors

Bashar Naji and Gaurav Sood