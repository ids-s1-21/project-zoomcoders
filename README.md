Economic Development Effect on Quality of Life
================
by zoomcoders

## Summary

For our project, we wanted to explore the relationships between economic
development and quality of life. Hence, our goal for this project was to
investigate how the development of a country can impact the quality of
life of its citizens. Quality of life was measured through health
related measurements for the most part. Our hypothesis for this project
was that “If we plot different measurements of quality of life against
development by country, we expect to see a positive linear relationship
because higher development leads to better quality of life”. To be more
specific, we expected measurements where higher values are desired such
as life expectancy to have a positive linear relationship with
development, and vice versa. For this project, we used multiple datasets
from two major databases: The UN Development Programme Human Development
Reports, and World Health Organization Global Health Observatory. We
then cleaned up the datasets, and then joined them altogether to make
one large dataset, having one observation for each measurement per
country. The data we used was from the year 2019, as this is the latest
year we could find information for all of the measurements we wanted to
use.

For the first part of our analysis, we chose to fit linear regressions
to different quality of life measurements against Human Development
Index (HDI). The reason we chose HDI for this particular analysis is
that it is a widely recognised measurement for development in a country,
which gave us a pretty reliable value for each country’s development. By
fitting linear regressions, we could firstly test our hypothesis and see
if all these “good” measurements had a positive linear relationship with
HDI, and “bad” measurements had a negative linear relationship with HDI.

For life expectancy, we saw a positive linear relationship, with a 3.6
year increase in life expectancy with an increase of 0.1 in HDI. The R
Squared value was 0.781. For births attended by skilled health
personnel, we saw a positive linear relationship as well, with a 9%
increase per 0.1 increase in HDI. The R Squared value was 0.56. For
infant mortality rate, we saw a negative linear relationship, with an
11.4% decrease per 0.1 increase in HDI. The R Squared value was 0.78.
With this process repeated, we saw a negative relationship for number of
maternal deaths and maternal mortality ratio, as well as for suicide
rates. However, the R Squared value for Suicide rates was very low at
0.02, indicating that a linear fit was not necessarily acceptable.

From the initial regression fits, we could see that our hypothesis was
mostly correct. We generally saw a linear relationship between our
measurements and HDI, seeing positive linear relationships with
measurements such as healthy life expectancy, births attended by skilled
health personnel, and negative linear relationships with measurements
such as suicide rate, number of maternal deaths, infant mortality rate,
and maternal mortality rate. However, the strength of these
relationships varied, as we saw that the r squared values of some of
these relationships was as high as 0.78, and some as low as 0.02. For
the next part of our analysis we want to see how the r squared values of
these measurements compare to each other. This would give us a better
understanding of what kinds of health measurements have strong
relationships with development.

From our adjusted r squared plot, we could see that variables such as
healthy life expectancy at birth and infant mortality rates had the
highest r squared values. We expect more developed countries to have
better medical facilities, therefore have longer healthy life
expectancies (strong positive relationship), and have lower rates of
infant mortality (strong negative relationship). However, we also saw
that certain measurements such as maternal deaths and suicide rate had
relatively low r squared values. For maternal deaths, this can be
explained by the fact that for HDI values higher than 0.8, number of
maternal deaths was almost zero, hence not fitting a linear model that
well. For suicide rate, we can infer that although medical facilities
and technology may be quite high, this does not necessarily relate to
high levels of mental health.

We can overall say that our hypothesis was backed up by our results.
However, the spread was much higher than expected. Highest r squared
value for any measurement was 0.78, indicating that there isn’t such a
straightforward linear relationship between a measurement and HDI. In
addition we saw that measurements such as suicide rate didn’t
necessarily have a strong relationship with HDI. This could be caused by
a multitude of other factors, that may be more present in countries that
are more developed. Example: stress caused by work, school, etc.
Overall, this analysis helped us to understand the correlation between
multiple measurements of health and quality of life with development in
countries. Whilst our hypothesis was generally backed up, we realised
that measurements more reliant on medical technology and availability
were more likely to have a strong correlation with development, as would
be expected.

## Presentation

Our presentation can be found
[https://media.ed.ac.uk/media/zoomcoders_project_IDS/1_5trwa9a3](presentation/presentation.html).

## Data

-   [HDI by country - 2019](http://hdr.undp.org/en/indicators/137506)
-   [Population living below poverty line (%) by country -
    2019](http://hdr.undp.org/en/indicators/39006)
-   [Current Health Expenditure (% of GDP) by country -
    2019](http://hdr.undp.org/en/indicators/18180)
-   [Maternity Mortality Ratio by country -
    2019](https://www.who.int/data/gho/data/indicators/indicator-details/GHO/maternal-mortality-ratio-(per-100-000-live-births))
-   [Suicide Rates by country -
    2019](https://www.who.int/data/gho/data/themes/mental-health/suicide-rates)
-   [Births attended by skilled personnel (%) by country -
    2019](https://www.who.int/data/gho/data/indicators/indicator-details/GHO/births-attended-by-skilled-health-personnel-(-))
-   [Healthy Life Expectancy by country -
    2019](https://www.who.int/data/gho/data/indicators/indicator-details/GHO/gho-ghe-hale-healthy-life-expectancy-at-birth)

## References

Human Development Reports, 2021, *Human Development Index (HDI)*,
electronic dataset, United Nations Development Programme, viewed 12
November 2021 <http://hdr.undp.org/en/indicators/137506>

Human Development Reports, 2021, *Population living below income poverty
line, national poverty line (%)*, electronic dataset, United Nations
Development Programme, viewed 12 November 2021
<http://hdr.undp.org/en/indicators/39006>

Human Development Reports, 2020, *Current health expenditure (% of
GDP)*, electronic dataset, United Nations Development Programme, viewed
12 November 2021 <http://hdr.undp.org/en/indicators/181806>

The Global Health Observatory, 2019, *Maternal mortality ratio (per 100
000 live births)*, electronic dataset, World Health Organization, viewed
12 November 2021,
<https://www.who.int/data/gho/data/indicators/indicator-details/GHO/maternal-mortality-ratio-(per-100-000-live-births)>

The Global Health Observatory, 2021, *Age-standardized suicide rates
(per 100 000 population)*, electronic dataset, World Health
Organization, viewed 12 November 2021,
<https://www.who.int/data/gho/data/themes/mental-health/suicide-rates>

The Global Health Observatory, 2021, *Births attended by skilled health
personnel (%)*, electronic dataset, World Health Organization, viewed 12
November 2021,
<https://www.who.int/data/gho/data/indicators/indicator-details/GHO/births-attended-by-skilled-health-personnel-(-)>

The Global Health Observatory, 2021, *Crude suicide rates (per 100 000
population)*, electronic dataset, World Health Organization, viewed 12
November 2021,
<https://www.who.int/data/gho/data/themes/mental-health/suicide-rates>

The Global Health Observatory, 2021, *Healthy life expectancy (HALE) at
birth (years)*, electronic dataset, World Health Organization, viewed 12
November 2021,
<https://www.who.int/data/gho/data/indicators/indicator-details/GHO/gho-ghe-hale-healthy-life-expectancy-at-birth>
