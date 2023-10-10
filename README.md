This project in an exploration into the factors that allow a specific data analysis to be reproducible.

## Project Goal 
The goal of this assignment is to construct, analyze, and publish a dataset of monthly article traffic for a select set of pages from English Wikipedia from July 1, 2015 through September 30, 2023. The learning objective is to create an analysis that can be reproduced and implemented by anyone who reads this repository and goes over the Python notebook. 

## Data Source
The dataset that has been used for this analysis - https://docs.google.com/spreadsheets/d/1A1h_7KAo7KXaVxdScJmIVPTvjb3IuY9oZhNV4ZHxrxw/edit#gid=1229854301.
Thehe Wikimedia Foundation REST API  was used to access pageview data for Wikipedia articles. The data spans from July 2015 through to the previous complete month.

## API Documentation
In order to measure article traffic from 2015-2023, data was collected from the Pageviews API. 
Documentation - https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews
Endpoint - https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end
Terms of use of the Wikimedia Foundation REST API - https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions
Further the following example notebook was used under the CC-BY license.
Example Notebook - https://drive.google.com/file/d/1XjFhd3eXx704tcdfQ4Q1OQn0LWKCRNJm/view
CC-BY License - https://creativecommons.org/licenses/by/4.0/
 
## Environment
Jupyter was used in order to run a .ipynb Notebook. Any editor that allows .ipynb notebooks can be used to run this project following the installation of the modules specified in the code.

## License
This project is open-source and follows the MIT License. You are free to use and modify the code following the terms of the MIT License.

## Steps you can Follow to reproduce this work:
1)	Import the necessary Python libraries.
2)	Run the Jupyter notebook which contains the code to retrieve the data from the google document and the APIs, preprocess it, upload it into the output files and create the necessary visualizations. 

## Errors handled
The parameter safe='' was added to the urllib.parse.quote function so that it is able to handle cases where the movie name contains a special character

## Output Files 
The project generates three JSON output files. No intermediate files were created.
academy_monthly_mobile_201507-202312.json: Monthly mobile access data.
academy_monthly_desktop_201507-202312.json: Monthly desktop access data.
academy_monthly_cumulative_201507-202312.json: Monthly cumulative data.





