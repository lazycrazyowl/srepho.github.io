Churn Analysis
========================================================

One of the more common tasks in Business Analytics is to try and understand consumer behaviour. By understanding the hope is that a company can better change this behaviour. In many industries it is more expensive to find a new customer then to entice an existing one to stay. This is usually known as "churn" analysis.

### Data Set

This data is taken from a telecommunications company and involves customer data for a collection of customers who either stayed with the company or left wihtin a certain period. <i>In many industries its often not the case that the cut off is so binary. Frequently it might be more likely that a client account lays dormant rather then getting explicitly closed - for example if the client only pays for usage. I will explain how to adjust for these situations latter in the piece.</i> This dataset is taken from [here] (http://www.dataminingconsultant.com/data/churn.txt) with descriptions of the data available [here] (http://www.sgi.com/tech/mlc/db/churn.names). This dataset also appears in the [C50 package]. (http://cran.r-project.org/web/packages/C50/index.html)

Lets load the required packages:


```r
library(plyr)
library(dplyr)
library(ggplot2)
library(reshape2)
library(caret)
```

You can also embed plots, for example:


