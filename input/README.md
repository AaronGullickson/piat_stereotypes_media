# Data Source Description

The dataset we will use for this project comes from the 2020 [American National Election Study](https://github.com/AaronGullickson/piat_stereotypes_media.git) (ANES). The ANES has been a long-standing high quality of study of the American electorate conducted every two years. It collects a variety of information on voting behavior, political ideology, and opinion.

From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. To load this dataset in R, you just need to run the setup code chunk in the full_report.Rmd R Markdown document. The name of the dataset in R is `anes`. 

* **stereo_black**: This variable is the sum of two separate questions respondents were asked. They were first asked to choose a scale from 1 (hard-working) to 7 (lazy) and then a scale from 1 (peaceful) to 7 (violent) to rank black people. Higher scores on this scale represent more stereotyped attitudes. This is the key dependent variable.
* **use_tv, use_newspaper, use_internet, use_radio**: These are a series of 1/0 variables indicating whether a respondent used (TV/newspaper, internet, radio) media to get information on the 2020 presidential election. A value of 1 indicates a yes and a zero indicates no. These categories are not mutually exclusive (i.e. a respondent could be 1 on all of them). Collectively, these are the key independent variables.
* **age**: The age of the respondent in years. This is the key contextual variable.
* **race**: The respondent's self-reported race in the categories of White, Latino, Black, Asian and Pacific Islander, Native American, and Multiple Races.
* **educ**: The respondent's level of education.
* **foreign_born**: A TRUE/FALSE variable indicating whether the respondent was foreign-born.
