# A2-hcds-hcc

## Introduction
In today's science it is more than ever of great importance to document research results in detail. In the field of Open Science it is also important to provide used data to enable reproducibility or replicability. Not only does this serve to make results comprehensible, but it also enables them to be challanged. It is the duty of every scientist to critically evaluate the work of others as well as own research. This project was created during the course "Human Centered Data Science" at the Freie Universität Berlin to train concepts of reproducibility and replicability. 

The goal of this research was to visualize the website traffic of the english wikipedia page between January 2008 and October 2020. Results are presented as a plot.

## Data and Results
The given folder structure in this project should provide clarity and easy of use. All fetched and processed data can be found in raw_data as .json files or clean_data as .csv respectively. Analysis of the given data was done with pandas and results are presented as a plot that can be found in the folder results.

## Used Software and API
This data used in this research was fetched by following APIs:
1. The Legacy Pagecounts API ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts), [endpoint](https://wikimedia.org/api/rest_v1/#/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)) provides access to desktop and mobile traffic data from December 2007 through July 2016.
2. The Pageviews API ([documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews), [endpoint](https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end)) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through last month.

The data was analysed with the following software:
```
jupyter = "^1.0.0"
python = "^3.6.1"
requests = "^2.24.0"
pandas = "^1.1.3"
ipykernel = "^5.3.4"
matplotlib = "^3.3.2"
```
To replicate the workflow, one can use the poetry script, given in the root folder. This will install all required dependencies. It is recommended to do this research on a unix system due to the fact that dependency installation may be troublesome on Windows due to different dependency installation processes.

In order to use this workflow, please ensure that you have a [Python][1] version greater or equal to `3.6.1`, a working installation of [Poetry][2] and [git][3] installed. The project setup is described in the following paragraph.

### Setup

1. Clone this repository (or use SSH) and move it into the repo root.
```
	git clone https://github.com/kuzniarz/A2-hcds-hcc.git
	cd A2-hcds-hcc
```
2. Install the dependencies in the repo root.
```
	poetry install
```
3. Create a subshell within the virtual environment by running:
```
	poetry shell
```
4. Open the project with Jupyter in your browser.
```
	jupyter notebook
```
## License
This project ist MIT licensed. Further information can be found in the LICENSE file.

---
[1]:  https://www.python.org/
[2]:	https://python-poetry.org/docs/
[3]:	https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
