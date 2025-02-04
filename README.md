## Introduction & Objective
My data set, acquired from the Ken French Data Library, included 25 portfolios ranked upon size and book-to-market ratio. The portfolios range across small-cap to large-cap stocks, varying from low book-to-market ratios (growth stocks) to high book-to-market ratios (value stocks) and are titled accordingly. In addition, we have the factor returns for all time periods, including RMRF (market risk premium), SMB (size factor), and HML (value factor). Along with my team, I performed the analysis for all 25 of these portfolios.

## CAPM TEST

CAPM is a strong theoretical framework developed in the 1960s by Sharpe, Litner, Mossin, and Treynor to explain the relationship between expected return and exposure to market risk. The model defines beta as a measure of an asset’s sensitivity to the market risk premium. With this 1-factor model, I will perform a series of empirical tests to assess the validity of the model. This is important given many concerns have been raised about the validity of CAPM. Many people still use the model to price assets due to its simplicity, but the weaknesses must also be highlighted

## Fama-French 3-Factor Model
The Fama-French 3-Factor Model (FF3F) was developed in the early 1990s by Fama and French and acts as an extension to CAPM. The model adds two additional factors, size and value, for a total of 3 factors used to explain the variability in stock returns. The size factor (SMB) captures the tendency for small-cap stocks to outperform large-cap stocks, and the value factor (HML) captures the tendency for firms with high book-to-market ratios to outperform firms with lower ratios. I can perform the same tests from the CAPM section to observe if the analysis will change with the inclusion of more factors.

## Using the Python Tool 

The tool queries the user for the data file (must include portfolio returns and factor data), and also asks them to provide a date range in YYYYMM format. We included input validation to make sure the data file exists, ensuring the number of periods is a positive integer, and that the start and end dates are formatted as expected. The program was written in an object-oriented method so all of the data is represented as attributes within a class. There are two different classes for CAPM and the FF3F model, with different functions to perform TSR, CSR, FMP, and the GRS F-Test. The model accounts for multiple time periods, so the user can select as many periods as are required. Afterwards, all the tests will be performed automatically. Finally, the tool writes to Excel so the user can view the results to assess the validity and usefulness of CAPM and Fama-French 3-Factor Model for predicting an asset’s expected return

## Conclusion 
All results from the regressions are posted in the excel file titles "Empirical_Testing_Results". While the FF3F model provides a more comprehensive framework than CAPM, the persistence of significant alphas in both models suggests that neither fully captures the sources of return variation across portfolios, particularly in recent decades. These findings emphasize the need for continued development and refinement of asset pricing models. Models have developed over time to include additional factors such as profitability, momentum, or investment, to better align with modern market dynamics and more accurately explain the cross-section of returns.



