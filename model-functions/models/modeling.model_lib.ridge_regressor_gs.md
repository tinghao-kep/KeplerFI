---
description: 'ridge_regressor_GS(X_train, y_train, X_test, y_test, hyperparams={}, cv=3)'
---

# model\_lib.ridge\_regressor\_GS

Performs ridge regression with cross-validated grid search. Finds the best 

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>Input</b>
      </td>
      <td style="text-align:left">
        <p><b>X_train, X_test </b>: pandas.DataFrame, or 2d numpy.array</p>
        <p></p>
        <p><b>y_train, y_test </b>: pandas.Series, or 1d numpy.array</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Parameters</b>
      </td>
      <td style="text-align:left">
        <p><b>hyperparams </b>: dict</p>
        <p>List of hyperparameter names and values. e.g. {&apos;lambda&apos;: 1,
          &apos;normalize&apos;: True}</p>
        <p>&lt;b&gt;&lt;/b&gt;</p>
        <p><b>cv </b>: int</p>
        <p>Number of folds in grid search cross-validation. A small number (&lt;=3)
          is recommended for small sample size.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Output</b>
      </td>
      <td style="text-align:left">
        <p><b>output </b>: dict</p>
        <p>Returns a dictionary of variables:</p>
        <ul>
          <li>&apos;y_pred&apos; - predicted values</li>
          <li>&apos;hyperparams&apos; - best set of parameters obtained from grid search</li>
          <li>&apos;r_squared&apos; - in sample r2</li>
          <li>&apos;feat_imp&apos; - feature importance of the best model</li>
          <li>&apos;coef&apos; - regression coefficients</li>
          <li>&apos;best&apos; - model object of the best model</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

