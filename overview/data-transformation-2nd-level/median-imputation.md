---
description: 'median_impute_col(series, days=90)'
---

# data.transform.median\_impute\_col

Performs rolling median imputation on a pandas series with datetime index.

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
        <p><b>series </b>: pandas.Series</p>
        <p>A series of values with a datetime index that is not necessarily unique</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>Parameters</b>
      </td>
      <td style="text-align:left">
        <p><b>days</b>: int</p>
        <p>Size of the moving window in days. It is possible to have much more or
          less observations than the window size. The default 90 days corresponds
          to approximately a quarter.</p>
      </td>
    </tr>
  </tbody>
</table>