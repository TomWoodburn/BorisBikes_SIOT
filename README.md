# BorisBikes_SIOT
Data Collection and an Interactive Web App that compares Boris Bike availability and the brightness of the day.

Completed Monday 13th January 2020

### 4 Important .zip files

1. BorisBikeData.zip
2. LightSensorData.zip
3. PreProcessing.zip
4. AppBuild.zip



#### 1. BorisBikeData.zip

Contains:

**data_downloader.sh**: Shell script that runs every 5 minutes in GitBash terminal. The script pulls the web address "Humbolt Road, Fulham" docking station (https://api.tfl.gov.uk/BikePoint/BikePoints_761), and saves it as a .json file to that day's destination folder, within the "JSON_data" folder path. 

**AllJsonFoldersToCSV.py**: All json folders are converted to one .csv file, where the important information is extracted in .Excel (example file is "ConvertedJsonData0501-1101.csv")

#### 2. LightSensorData.zip

Contains:

**SIOT_Lux_Test_2612.ino**: Arduino script that processed data from the light sensor, the sensor data was saved in a PLX-DAQ Macro enabled Excel document.

**LightDataAll.Excel**: Manually processed daily upkeep of sensor data

#### 3. PreProcessing

contains: 

**0501-1101 PreProcessing Data.Excel**: Data was cleaned, averages, standardization of data; and output of clean .cvs files that could be read for the web app

#### 4. AppBuild

**3 .cvs files**: Converted into Panda data frames within the app

**app.py**: The script to run the web app "Boris on a Bike"

**Correlation.py**: Supplementary processing of data













