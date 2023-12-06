The platooning drag reduction model in [1] lists incorrect coefficients in Table 1.
As a result the model cannot be used. 
In this project, I used WebPlotDigitizer to reconstruct the coefficients in Table 1 of [1].

| Source      | $X_1$       | $X_2$       | $X_3$       | $X_4$       | $X_5$       | $X_6$       |
| ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| Published   | 0.1821      | 1.5216      | 0.6643      | 8.9340      | 0.3371      | -0.0419     |
| Recalculated| 5.4543      | 1.5197      | 0.6610      | 8.9289      | 0.3374      | -0.0422     |

It appears that only the coefficient $X_1$ was misstated in the publication. 
However, each coefficient is dependent on the last ones due to the model formulation.
Rather than using only the recalculated $X_1$ and the original coefficients $X_2$&mdash;$X_6$, I recommend using the recalculated values.

The MATLAB code for constructing the values is given in the pdf.

Sources:

[1] Schmid, M. et al. (2020) ‘Prediction Model for Energy Consumption in Heavy-Duty Vehicle Formations’
