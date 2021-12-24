---
title: "Assisted Living in the United States: an Open Dataset"
# date: 2021-11-17T15:00:42-05:00
draft: false
author: ""
---

This website contains the first public dataset of assisted living facilities in the United States, covering over 44,000 facilities from all 50 states and the District of Columbia.

[Here](https://github.com/onefact/assisted-living/blob/main/assisted-living-facilities.csv) is the dataset (13MB) as a CSV. [Here](https://github.com/onefact/assisted-living) is the github repo, which contains all scripts used to process, clean, and analyze the data, as well as all raw data gathered from state licensing agencies.

The data was collected over the course of summer 2021. The dataset---along with a conceptual replication of previous work and a geospatial analysis of assisted living accessibility---was accepted at NeurIPS 2021 as part of the [Machine Learning in Public](https://sites.google.com/nyu.edu/mlph2021/home) (MLPH) workshop.

[Here](https://drive.google.com/file/d/1lqGBlq93fJXXHLCkbn_c6bjd_-AAs6e3/view?usp=sharing) is the preprint paper.

If you have any questions, feel free to reach out to [Anton Stengel](https://www.linkedin.com/in/anton-stengel-339179147/) at:

 *astengel* at *princeton* dot *edu*.

### Background about dataset

{{< embed-pdf url="./al-graph.pdf" >}}

Since assisted living facilities are not federally regulated, there is no standardized definition of what constitutes a facility. We followed the NCAL's [2019 Assisted Living
State Regulatory Review](https://www.ahcancal.org/Assisted-Living/Policy/Documents/2019_reg_review.pdf) to define which licensing types count for each state. We collected data by 

1. retrieving CSVs and PDFs from state websites
1. scraping data from state websites 
1. directly contacting state licensing agencies
1. submitting Freedom of Information Act requests


Here are the variables for each facility instance. The **Percent Filled** column specifies what percent of facilities in the dataset contain the relevant variable.

| Variable                                  | Description                                                  | Percent Filled |
|-------------------------------------------|--------------------------------------------------------------|----------------|
| Facility Name                             | The name of the facility                                     | 100%           |
| Facility ID                               | The facility identification number                           | 65%            |
| License Number                            | The facility license number                                  | 48%            |
| Address                                   | The primary physical address of the facility                 | 100%           |
| City                                      | The city of the address                                      | 98%            |
| State                                     | The state of the address                                     | 100%           |
| Zip Code                                  | The zip code of the address                                  | 97%            |
| County                                    | The county of the address                                    | 100%           |
| County FIPS                               | The FIPS code of the county                                  | 100%           |
| Latitude                                  | Latitude of the address                                      | 100%           |
| Longitude                                 | Longitude of the address                                     | 100%           |
| Facility Type Primary                     | The primary licensing type of the facility                   | 100%           |
| Facility Type Secondary                   | The secondary licensing type of the facility                 | 41%            |
| Capacity                                  | The total capacity of the facility in beds                   | 86%            |
| Ownership Type                            | The ownership structure of the facility                      | 27%            |
| Licensee                                  | The license holder of the facility                           | 48%            |
| Phone Number                              | Primary phone number associated with facility                | 98%            |
| Email Address                             | Primary email address associated with facility               | 35%            |
| Date Accessed                             | Date that the data was retrieved from state licensing agency | 100%           |
| Total County AL Need                      | The computed need-based metric for county of facility        | 100%           |
| County Percent of Population 65 or Older  | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Median Age                         | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Homeownership Rate                 | Retrieved from 2015-2019 ACS data                            | 100%           |
| County College Education or Higher Rate   | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Percent Black Population           | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Median Home Value of Owned Homes   | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Percent Hispanic Population        | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Percent of Population 85 or Older  | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Medan Household Income             | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Unemployment Rate                  | Retrieved from 2020 ACS data                                 | 100%           |
| County Less Than High School Diploma Rate | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Percent Whilte Population          | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Gender Ratio                       | Retrieved from 2015-2019 ACS data                            | 100%           |
| County Poverty Rate                       | Retrieved from 2015-2019 ACS data                            | 100%           |





