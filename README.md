# practiceprojectwkhaled

Import Los Angeles Crime Data set 

Prepare data set:

1) remove unnessary columns : Date Rptd, TIME OCC, Part 1-2, Mocodes, Crm Cd1, Crm Cd2, Crm Cd3, Crm Cd4, Cross Street

2) removed year 2023 records since it's only up to date of 10-2023

3) remove missing values rows in column Vict Descent, Premis Desc

4) replace blanks values in column Weapon Used Cd, and Weapon Desc with N/A


Below are all the variables in the dataset, followed by its description:

* DR_NO (Division of Records Number): Official file number made up of a 3 digit year, area ID, and 5 digits.

* DATE OCC (Date of crime occurrence): (YYYY-MM-DD)

* AREA: The LAPD has 21 Community Police Stations referred to as Geographic Areas within the department. These Geographic Areas are sequentially numbered from 1-21.

* AREA NAME: The 21 Geographic Areas or Patrol Divisions are also given a name designation that references a landmark or the surrounding community that it is responsible for.

* Rpt Dist No: Code that represents a sub-area within a Geographic Area.

* Crm Cd: Indicates the crime committed.

* Crm Cd Desc: Defines the Crime Code provided.

* Vict Age: Indicates the age of the victim.

* Vict Sex:
    * F: Female 
    * M: Male 
    * X: Unknown
    * H: Male
    
* Vict Descent (Descent Code): 
    * A: Other Asian 
    * B: Black 
    * C: Chinese 
    * D: Cambodian 
    * F: Filipino 
    * G: Guamanian 
    * H: Hispanic/Latin/Mexican 
    * I: American Indian/Alaskan Native 
    * J: Japanese 
    * K: Korean 
    * L: Laotian 
    * O: Other 
    * P: Pacific Islander 
    * S: Samoan 
    * U: Hawaiian 
    * V: Vietnamese 
    * W: White 
    * X: Unknown 
    * Z: Asian Indian
    
* Premis Cd: The type of structure, vehicle, or location where the crime took place.

* Premis Desc: Defines the Premise Code provided.

* Weapon Used Cd: The type of weapon used in the crime. there are total of 80 different types of weapon used include blank, need to replace blank with "N/A"

* Weapon Desc: Defines the Weapon Used Code provided.

* Status Desc with code:
    * AO: Adult Other 
    * IC: Inves Cont
    * JA: Juv Arrest
    * JO: Juv Other
    * AA: Adult Arrest
    

* LOCATION: Street address of crime incident rounded to the nearest hundred block to maintain anonymity.

* LAT: Latitude Coordinate.

* LON: Longitude Coordinate.