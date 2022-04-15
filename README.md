# Seattle_Crime_Data

Seattle Crime Data Analysis. In this Project I used Seattle crime data to do exploratory analysis and provide statistical answers to the issues. 
Dataset contains the following columns: Report Number: Unique report number for the record. 
Offense Id : When a single report contains several violations, a unique identification is used to indicate this.
Offense Start DateTime: Offense start time and date.
Offense End DateTime: End date and time of offense.
Report DateTime: Date and time the offenses was reported.
Group A B: offense group
Crime Against Category: offense crime of each category.
Offense Parent Group: Parent group of offense.
Offense: Crime or offense reported.
Offense Code: Code of offense
Precinct: Where the offenses occurred is indicated with a police precinct boundary.
Sector: Where the offenses happened, a police sector boundary was designated.
Beat: Designated police sector boundary where offense(s) occurred.
MCPP:Where the offenses happened, there is a designated Micro-Community Policing Plans (MCPP) boundary.
100 Block Address:The location of the offenses has been obfuscated to the hundred block.
Longitude: The spatial coordinates of the offenses were blurred to the hundred block.
Latitude: The spatial coordinates of the offenses have become hazy up to the hundred block.

DATASET SOURCE:
https://data.seattle.gov/Public-Safety/SPD-Crime-Data-2008-Present/tazs-3rd5/data

Project Implementation:
Exploratory Data Analysis:
1)I have changed the name of the columns for easy use.
2)Checking missing and null values and replacing the Nan values if neccessary with approriate value.
3)Dropping the uneccessary columns and checked for duplicate values.
4)Changing the Datatypes to correct type.
5)Performed visualizations based of 
