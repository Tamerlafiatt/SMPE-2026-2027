\# Challenger — MOOC RR Module 2, Exercise 5



\## Objective



Study the relation between temperature and O-ring incidents, and evaluate the quality of the visualizations.



\## 1. Expected incidents vs temperature



!\[Expected incidents](images/expected\_incidents.png)



This is a good visualization.



The relationship is easy to see: lower temperatures are associated with more incidents.



The labels for the Binary and Binomial curves are useful.



Different colors or line styles could make the two curves easier to distinguish.



\## 2. O-ring thermal-distress table



!\[O-ring table](images/table1.png)



The table contains a lot of information, but you almost need to be a \*\*rocket scientist\*\* to understand all the technical terms.



A simpler table with only the main variables, such as temperature, pressure and number of incidents, would be easier to read.



\## 3. Graphs with and without zero incidents



!\[Incidents comparison](images/incidents\_comparison.png)



The first graph shows only flights with incidents.



The second graph is better because it also includes flights with zero incidents.



This makes the relationship between temperature and incidents much clearer.



It also shows why we should not ignore zero-incident flights.



\## 4. Erosion / Blowby graph



!\[Erosion and blowby](images/erosion\_blowby.png)



This graph is difficult to understand.



The symbols `+` and `#` are not clearly explained, and there is no clear chart key.



I would use different colors and shapes with a legend.



The y-axis scale could also be cleaner because the indicator is basically around 0 or 1.



\## 5. Binomial-logit model



!\[Binomial logit](images/binomial\_logit.png)



This graph is clear and well chosen.



It shows that the expected number of incidents increases when temperature decreases.



The main trend is easy to understand.



The meaning of the different curves could be explained more clearly.



\## Conclusion



The main lesson is that visualization choices can strongly affect interpretation.



Including all observations, especially flights with zero incidents, gives a much clearer view of the relationship between temperature and O-ring problems.



\## Results of the corrected analysis



The original analysis removes flights with zero O-ring incidents.



This is the main problem because these flights contain important information.



Using all 23 launches, the fitted logistic regression gives:



\- Temperature coefficient: \*\*-0.1156\*\*

\- p-value: \*\*0.014\*\*



Therefore, temperature has a significant effect on O-ring malfunction:



\*\*Lower temperatures are associated with a higher probability of failure.\*\*



Some estimated probabilities of malfunction for one O-ring are:



| Temperature | Estimated probability |

|-------------|----------------------:|

| 75°F | 2.7% |

| 70°F | 4.7% |

| 57°F | 18.2% |

| 53°F | 26.1% |

| \*\*31°F\*\* | \*\*81.8%\*\* |



At Challenger's planned launch temperature of \*\*31°F\*\*, the model predicts a very high malfunction probability.



However, 31°F is outside the range of the previous launch temperatures, so this prediction is an extrapolation and has high uncertainty.



The main mistake in the original analysis was therefore excluding the zero-incident launches.



Once all observations are included, the effect of temperature becomes much clearer.

