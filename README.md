# PROJECT1 - An analysis on Airbnb data
* The project aims to run an analysis on available Airbnb data in hopes to identify investment opportunities in the Inner Melbourne suburbs and help people decide where to establish first listings.


## CONTRIBUTORS:
**JASON SUTTON**<br>
**LINDA LEVY**<br>
**RAPHAEL SERRANO**<br>
**SWOBABIKA JENA**<br>


## HYPOTHESES:
* **Proximity to the CBD will increase earnings**
* **Train proximity will increase earnings**
* **Neighbourhoods with the highest earnings are the most popular areas**
* **The popularity of property types will be reflected in higher earnings**


## NAVIGATING THE REPOSITORY:

### 01-Project_Documents
* Contains all the documents and image files for the project
    - **/01-Project_Documents/Work_Plan_Based_on_Proposal_15012021.docx**
    - **/01-Project_Documents/0Airbnb Invesment Write Up.docx**
#### /01-Project_Documents/01-Presentation_Slides
+ Contains the presentation slides and the following subfolders for image output:
    - **/01-Project_Documents/01-Presentation_Slides/Correlation_Output**
    - **/01-Project_Documents/01-Presentation_Slides/Occupancy_Analysis**
    - **/01-Project_Documents/01-Presentation_Slides/Price_Output**
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
*The jupyter notebooks under "03-Project_Jupyter_Notebooks" directory are numbered in sequence, 01 and 02 are required to be ran consecutively but the other notebooks can be executed any time.*

* **00_Prelim_Data_Cleanup_Test_JS.ipynb** - This notebook was utilised for testing the cleanup logic which was later applied to "01_Data_Cleanup.ipynb"<br>
***DATA REFERENCED:***<br>
IN: "../02Data_Files_Directory/01Raw_Data/listings_2018_DataIssueCLean_15012021_JS.csv"

* **01_Data_Cleanup.ipynb** - This notebook contains the cleanup and data cutdown logic for the chosen categories. This also contains the first logic for the Haversine formula which was utilised to get the distance from CBD based on coordinates and filterwithin 12km.<br>
***DATA REFERENCED:***<br>
IN: "../02-Data_Files_Directory/01-Raw_Data/listings_2018_prelimClean_JS.csv"<br>
OUT: "../02-Data_Files_Directory/02-Clean_Data/airbnbFINAL_JS.csv"<br>
OUT: "../02-Data_Files_Directory/02-Clean_Data/airbnbFINAL_Swobabika.csv"<br>


* **02_Calculate_Nearest_Station.ipynb** - This notebook contains the logic to get the nearest station based on the latitude and longitude also utilising the Haversine formula. This will add the nearest station and distance to the main data. <br>
***DATA REFERENCED:***<br>
IN: "../02Data_Files_Directory/02Clean_Data/ptv_metro_train_station.csv"<br>
OUT: "../02Data_Files_Directory/02Clean_Data/airbnbFINAL_Swobabika.csv"

* **03_Price_Analysis.ipynb** - This notebook was utilised to perform price analysis and ranking for each suburb. Outliers are also identified in the process.<br>
***DATA REFERENCED:***<br>
IN: "../02Data_Files_Directory/02Clean_Data/airbnbFINAL_Swobabika.csv"

* **04_Correlation_Analysis.ipynb** - This notebook runs scatter and line plots to determine correlation between data fields for the significance tests with the hypotheses.<br>
***DATA REFERENCED:***<br>
IN: "../02Data_Files_Directory/02Clean_Data/airbnbFINAL_Swobabika.csv"

* **05_Airbnb_Occupancy_Analysis_JS.ipynb** - This notebook is responsible for running analysis on occupancy and rankings based on suburbs and property types<br>
***DATA REFERENCED:***<br>
IN: "../02Data_Files_Directory/02Clean_Data/airbnbFINAL_JS.csv"

* **06_Airbnb_Occupancy_Analysis_CSVSwob_JS.ipynb** - This notebook is a more comprehensive version of 05_Airbnb_Occupancy_Analysis_JS.ipynb which utilise the final data. <br>
***DATA REFERENCED:***<br>
IN: "../02Data_Files_Directory/02Clean_Data/airbnbFINAL_Swobabika.csv"

