# Cumulative Risks of Solitary Confinement

Hannah Pullen-Blasnik (hannah.pullen-blasnik@columbia.edu)

09/21/2021

This code provides documentation for the paper "The Population Prevalence of Solitary Confinement" by Hannah Pullen-Blasnik, Jessica T. Simes, and Bruce Western.

Per our data use agreement, data used in this analysis is not publicly available. Requests may be made for data access following a material transfer agreement to bruce.western@columbia.edu and simes@bu.edu.

This archive contains the following files:

--

### Code

data\_cleaning.Rmd: R code for cleaning raw data downloads for population, migration, and mortality, as well as initial cleaning on PA DOC misconduct ticket data for the 1986-1989 birth cohort admitted between 2007 and 2016. 

lifetable.Rmd: R code for combining the cleaned data on population, migration, mortality, and solitary confinement using lifetable methodology to estimate the population prevalence of incarceration and solitary confinement for the birth cohort, for varying minimum durations of solitary confinement up to one year.

tables\_figures.Rmd: R code for creating the tables and figures present in the paper, based on the output from the lifetable estimates and the raw PA DOC birth cohort data.

--

### Data

#### External Data

sc-est2019-alldata6.csv: state population estimates by year and age (ACS: https://www.census.gov/data/tables/time-series/demo/popest/2010s-state-detail.html)

bc\_census\_pop\_est.csv: state population estimates filtered to Pennsylvania, cleaned and aggregated

pa\_mortality\_data.csv: mortality by age, race, and gender (CDC: https://wonder.cdc.gov/controller/datarequest/D76;jsessionid=6AA4D02724C6A57536EFE9ADF294F040)

usa\_00001.csv: state-level migration by year, age, race, and gender (IPUMS: https://usa.ipums.org/usa-action/data_requests/download)

#### Aggregates

bc\_pop\_avg.csv: PA state population estimates for ages 18-32 by race and gender.

migration.csv: PA state outmigration estimates for ages 18-32 by race and gender.

mortality.csv: PA mortality rate for ages 18-32 by race and gender.

example\_incarcerated.csv: PA DOC example summary data for the average number of people incarcerated per year of age in the 1986-1989 birth cohort by race and gender.

example\_solitary.csv: PA DOC example summary data for the average number of people held in solitary confinement for at least 1 day by year of age in the 1986-1989 birth cohort by race and gender.

#### Output

incar\_lf\_20200825.csv: Lifetable output estimates of age-specific risk, cumulative risk, and population prevalence for incarceration by age, race, and gender for ages 18-30 in the 1986-1989 birth cohort.

solitary\_durations.csv: Lifetable output estimates of age-specific risk, cumulative risk, and population prevalence for solitary confinement by age, race, gender, and length of stay in solitary confinement for ages 18-30 in the 1986-1989 birth cohort.

--

birthyear\_scalars.csv: Scaling reference table to standardize population estimates by years of the birth cohort observed at a given age.


Data that cannot be included in this zip file consists of the PA DOC misconduct ticket level data for the birth cohort born 1986-1989 and admitted 2007-2016. Please use example summary files example\_incarcerated and example\_solitary, or contact the authors for more information on data transfer agreements. 
