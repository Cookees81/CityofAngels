# CityofAngels

Database summary:
-------------------------------------------------------------
This dataset reflects incidents of crime in the City of Los Angeles dating back to 2020. This data is transcribed from original crime reports that are typed on paper and therefore there may be some inaccuracies within the data. Some location fields with missing data are noted as (0°, 0°). Address fields are only provided to the nearest hundred block in order to maintain privacy. 

Website: https://catalog.data.gov/dataset/crime-data-from-2020-to-present

--------------------------------------------------------------

Contributors to Dataset Analysis:
---------------------------------------------------------------
- Thanos Chryssis (github.com/surfaki)
- Yee Wai Huang (github.com/sentvivi)
- Leslie Leiva (github.com/lleiva25)
- Teresa Salazar (github.com/Cookees81)
- Steve Islava (github.com/steve_islava)


---------------------------------------------------------------
Analysis Of Dataset
---------------------------------------------------------------
The top 3 committed crime areas are 77th Street, Central, Devonshire
- The highest-density crime areas are Central and Hollywood
- Crime drop between Mar 2020 and June 2021 aligns with CA Covid restrictions
- No large difference between male and female victims
- The age group mostly affected is 26 to 45. 
- Only 10% of the crime is using deadly weapons and 60% is a weaponless crime
- Three main trafficking corridors at Sepulveda Blvd, Western Ave, and Figueroa St
- Daily crime peaks at noon and dips between the hours of 3 a.m. to 8 am
- The very high percentage of child sexual abuse affects females over the age of 13
- High Burglary count on white population over the age of 65, potentially due to high net worth discrepancy in the LA area between races
- When it comes to gender, there isn’t a significant difference between crimes focusing on  males and females aside from sexual crimes, which are less frequent

---------------------------------------------------------------
Import Los Angeles Crime Data set:
---------------------------------------------------------------
Prepare data set:

remove unnecessary columns: Date Rptd, TIME OCC, Part 1-2, Mocodes, Crm Cd1, Crm Cd2, Crm Cd3, Crm Cd4, Cross Street

removed year 2023 records since it's only up to date of 10-2023

remove missing values rows in column Vict Descent, Premis Desc

replace blanks values in column Weapon Used Cd, and Weapon Desc with N/A

Below are all the variables in the dataset, followed by its description:

DR_NO (Division of Records Number): Official file number made up of a 3-digit year, area ID, and 5 digits.

DATE OCC (Date of crime occurrence): (YYYY-MM-DD)

AREA: The LAPD has 21 Community Police Stations referred to as Geographic Areas within the department. These Geographic Areas are sequentially numbered from 1-21.

AREA NAME: The 21 Geographic Areas or Patrol Divisions are also given a name designation that references a landmark or the surrounding community that it is responsible for.

Rpt Dist No: Code that represents a sub-area within a Geographic Area.

Crm Cd: Indicates the crime committed.

Crm Cd Desc: Defines the Crime Code provided.

Vict Age: Indicates the age of the victim.

Vict Sex:

F: Female
M: Male
X: Unknown
H: Male
Vict Descent (Descent Code):

A: Other Asian
B: Black
C: Chinese
D: Cambodian
F: Filipino
G: Guamanian
H: Hispanic/Latin/Mexican
I: American Indian/Alaskan Native
J: Japanese
K: Korean
L: Laotian
O: Other
P: Pacific Islander
S: Samoan
U: Hawaiian
V: Vietnamese
W: White
X: Unknown
Z: Asian Indian
Premis Cd: The type of structure, vehicle, or location where the crime took place.

Premis Desc: Defines the Premise Code provided.

Weapon Used Cd: The type of weapon used in the crime. there are a total of 80 different types of weapons used include blank, which need to be blank with "N/A"

Weapon Desc: Defines the Weapon Used Code provided.

Status Desc with code:
AO: Adult Other
IC: Inves Cont
JA: Juv Arrest
JO: Juv Other
AA: Adult Arrest

LOCATION: The street address of the crime incident was rounded to the nearest hundred block to maintain anonymity.
LAT: Latitude Coordinate.
LON: Longitude Coordinate.

--------------------------------------------------------------

Analysis Impact & Limitations:
---------------------------------------------------------------
- Based on our dataset, our team wanted to provide crime statistics in order to identify areas of risk to those who are visiting LA.

- The dataset that was provided had no statistics of the time allocated per case or perpetrator information allowing us to only analyze from a victim’s perspective. 

- Data analysis could be improved by having access to API products that use coordinates in DataBase to plot graphs against census information such as Geocoding.

- If time allows, our team could spend more time analyzing which crime category has the highest closed case rate. This could impact LAPD agendas.

- Follow up with cross-analysis of other datasets to determine the correlation 
