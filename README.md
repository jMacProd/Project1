# PROJECT1 - An analysis on Airbnb data
* The project aims to run an analysis on available Airbnb data in hopes to identify investment opportunities in the Inner Melbourne suburbs and help people decide where to establish first listings.


## CONTRIBUTORS:
### JASON SUTTON
### LINDA LEVY
### RAPHAEL SERRANO
### SWOBABIKA JENNA


## HYPOTHESES:
* **Proximity to the CBD will increase earnings
* **Train proximity will increase earnings
* **Neighbourhoods with the highest earnings are the most popular areas
* **The popularity of property types will be reflected in higher earnings


## NAVIGATING THE REPOSITORY:

### 01-Project_Documents
* Contains all the documents and image files for the project
#### /01-Project_Documents/01-Presentation_Slides
* Contains the presentation slides and the following subfolders for image output:
##### /01-Project_Documents/01-Presentation_Slides/Correlation_Output
##### /01-Project_Documents/01-Presentation_Slides/Occupancy_Analysis
##### /01-Project_Documents/01-Presentation_Slides/Price_Output
#### /01-Project_Documents/02-Image_Files
* Contains screenshots for the initial analysis

### 02-Data_Files_Directory
* Contains all the data utilised in the analysis
#### /02-Data_Files_Directory/01-Raw_Data
* Contains the raw and pre-processed data
#### /02-Data_Files_Directory/02-Clean_Data
* Contains the data after finalising the criteria and running cleanup
#### /02-Data_Files_Directory/03-Other_Data
* Contains other data used in pre-analysis

### 03-Project_Jupyter_Notebooks
* Contains all the Jupyter Notebooks created for the project


## NOTEBOOK DESCRIPTIONS:
*The jupyter notebooks under "03-Project_Jupyter_Notebooks" directory are numbered in sequence, 01 and 02 are required to be ran consecutively but the other notebooks can be executed any time.

* **00_Prelim_Data_Cleanup_Test_JS.ipynb** - This notebook was utilised for testing the cleanup logic which was later applied to "01_Data_Cleanup.ipynb"

* **01_Data_Cleanup.ipynb** - This notebook contains the cleanup and data cutdown logic for the chosen categories. This also contains the first logic for the Haversine formula which was utilised to get the distance from CBD based on coordinates and filterwithin 12km.

* **02_Calculate_Nearest_Station.ipynb** - This notebook contains the logic to get the nearest station based on the latitude and longitude also utilising the Haversine formula. This will add the nearest station and distance to the main data. 

* **03_Price_Analysis.ipynb** - This notebook was utilised to perform price analysis and ranking for each suburb. Outliers are also identified in the process.

* **04





