if (!require('WDI', 'dplyr')) install.packages('WDI', 'dplyr'); library('WDI', 'dplyr')

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
