# Covid19-cases-deaths-vax-in-US-counties
The repository containst a jupyter notebook which helps you analyse COVID19 cases or deaths in given period against vaccination percentage (either fully vaccinated or with booster shot) in counties in USA.


The data about cases, deaths and population of counties is aquired from USA FACTS [https://usafacts.org/visualizations/coronavirus-covid-19-spread-map/]. The data about vaccination in counties is aquired from CDC, Centers for Disease Control and Prevention [https://data.cdc.gov/Vaccinations/COVID-19-Vaccinations-in-the-United-States-County/8xkx-amqh]. The data file with the land area information in counties uis aquired from OpenIntro [https://www.openintro.org/data/?data=county_complete]. You must download the data and put it in the `input_data` folder of the repository.

#### In the notebooks, you can choose the period you want to analyse and the maximum and minimum population size of the counties to be taken into consideration. The plots will be saved in `figures` directory.

In `Vax_cases_deaths` notebook the data for a given period is being collected. You specify the period in the file. You can look at the plots of infection waves and see which period you want to analyse. The file with all the data will be generated as `data/vax_cases_deaths.csv`.

You can use `readable_data_table` notebook to generate a table with formatted data and only most important information (which are 'countyFIPS', 'County Name', 'State', 'Population', 'Land Area in square miles','Pop. Density', 'Cases in given period', 'Deaths in given period', 'Percentage of fully vaccinated', 'Percentage of vaccinated with booster'). You can choose there the name of the file, you want to save the data in.

In notebook `display_plots_covid_data` you can generate figures which will be saved in `figures` directory. You can specify the minimum and maximum population and then the filtered data will be displayed on the plot. You can specify the beginning of the period and end (as you did in `Vax_cases_deaths` notebook) or pick a custom name. The information will appear in the filename of the figures.

