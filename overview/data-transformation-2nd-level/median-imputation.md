---
description: "DataFrame.rolling(self,\_window,\_min_periods=None,\_center=False,\_win_type=None,\_on=None,\_axis=0,\_closed=None)"
---

# Median Imputation

Provide rolling window calculations.

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>Parameters</b>
      </td>
      <td style="text-align:left">
        <p><b>window</b> : int, or offset</p>
        <p>Size of the moving window. This is the number of observations used for
          calculating the statistic. Each window will be a fixed size.</p>
        <p>If its an offset then this will be the time period of each window. Each
          window will be a variable sized based on the observations included in the
          time-period. This is only valid for datetimelike indexes. This is new in
          0.19.0</p>
        <p>&lt;b&gt;&lt;/b&gt;</p>
        <p><b>min_periods</b> : int, default None</p>
        <p>Minimum number of observations in window required to have a value (otherwise
          result is NA). For a window that is specified by an offset, min_periods
          will default to 1. Otherwise, min_periods will default to the size of the
          window.</p>
        <p>&lt;b&gt;&lt;/b&gt;</p>
        <p><b>center</b> : bool, default False</p>
        <p>Set the labels at the center of the window.</p>
        <p>&lt;b&gt;&lt;/b&gt;</p>
        <p><b>win_type</b> : str, default None</p>
        <p>Provide a window type. If <code>None</code>, all points are evenly weighted.
          See the notes below for further information.</p>
        <p>&lt;b&gt;&lt;/b&gt;</p>
        <p><b>on</b> : str, optional</p>
        <p>For a DataFrame, a datetime-like column on which to calculate the rolling
          window, rather than the DataFrame&#x2019;s index. Provided integer column
          is ignored and excluded from result since an integer index is not used
          to calculate the rolling window.<b>axis</b> : int or str, default 0</p>
        <p>&lt;b&gt;&lt;/b&gt;</p>
        <p><b>closed</b> : str, default None</p>
        <p>Make the interval closed on the &#x2018;right&#x2019;, &#x2018;left&#x2019;,
          &#x2018;both&#x2019; or &#x2018;neither&#x2019; endpoints. For offset-based
          windows, it defaults to &#x2018;right&#x2019;. For fixed windows, defaults
          to &#x2018;both&#x2019;. Remaining cases not implemented for fixed windows.</p>
        <p></p>
        <p>New in version 0.20.0.</p>
      </td>
    </tr>
  </tbody>
</table>