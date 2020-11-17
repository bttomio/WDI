if (!require('WDI', 'dplyr', 'ggplot2', 'ggthemes', 'knitr', 'kableExtra', 'rnaturalearth', 'tidyverse')) 
  install.packages('WDI', 'dplyr', 'ggplot2', 'ggthemes', 'knitr', 'kableExtra', 'rnaturalearth', 'tidyverse'); 
library('WDI', 'dplyr', 'ggplot2', 'ggthemes', 'knitr', 'kableExtra', 'rnaturalearth', 'tidyverse')

# Search for "GDP"
WDIsearch('GDP')

# Save results for "GDP"
GDP_search <- WDIsearch('GDP')

library(dplyr)

Data_info <- WDI_data

Data_series <- as.data.frame(Data_info$series) %>%
  filter(indicator == "NY.GDP.PCAP.KD")

Data_countries <- as.data.frame(Data_info$country) %>%
  filter(country == "Senegal")

# Search for "unemployment"
WDIsearch('unemployment')

# Save results for "unemployment"
UNEMP_search <- WDIsearch('unemployment')

indicator <- c("Unemployment" = 'UNEMPSA_')
datW <- WDI(indicator, country="all",start = '2020M02', end = '2020M02')

# Search for "life"
WDIsearch('life')

# Save results for "life"
life_search <- WDIsearch('life')

indicator <- c("Life expectancy at birth, female (years)" = 'SP.DYN.LE00.FE.IN')
datW <- WDI(indicator, country="all",start = '2018', end = '2018')

