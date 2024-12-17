# Data for: Age, sex, and temperature shape within- and among-individual space use in Black-capped Chickadees

[https://doi.org/10.5061/dryad.47d7wm3pn](https://doi.org/10.5061/dryad.47d7wm3pn)

## Description of the data and file structure

## Data description

This data was collected from January 9 to February 28, 2023 (inclusive). It contains feeder visit data from a marked population of Black-capped Chickadees (*Poecile atricapillus*).

### Files and variables

#### File: data\_AllDates.csv

**Description:** This file contains all data collected from January 9 to February 28, 2023 (inclusive), but excludes February 15 to February 23, 2023 (inclusive).

##### Variables

* VisitDate: date of observation (YYYY-MM-DD)
* TransponderHexCode: unique 10-digit hexadecimal PIT tag code
* UniqueFeederCount: the number of unique feeders visited by the bird on the given VisitDate
* AvgTemp: mean daily temperature in degrees Celcius
* Temp_stnd: the standardized temperature used in the analysis. Temperature was standardized by dividing values by 2 standard deviations so that the estimated effect of temperature reflects the effect of 1 s.d. change in temperature (i.e., 5.74°C).
* Sex: determined molecularly or by discriminant function score. Male or Female
* AgeBin: the binned age of birds (0 = birds hatched in 2022, “juveniles”; 1 = birds hatched in 2021 or earlier, “adults”)
* Age_Sex: a composite variable specifying the age (0 = juvenile or 1 = adult) and sex (male or female) of each individual, resulting in four levels (0Male, 0Female, 1Male, 1Female).
* VisitCount: the number of visits the bird made to feeders throughout the study site on the given VisitDate (i.e., daily feeding rate).
* Age: the minimum age of a bird with reference to their hatch year. The birds present in our study ranged in minimum age from 0 years (i.e., hatched in spring 2022) to 6 years (i.e., hatched in spring 2016 or earlier).

#### File: THC\_Survival.csv

**Description:** This file contains data on the annual survival of birds that used the feeders in Winter 2023.

##### Variables

* TransponderHexCode: unique 10-digit hexadecimal PIT tag code
* Survived: was a bird detected at our RFID-equipped feeders in Fall 2023 (i.e., did it survive?) (0 = no, 1 = yes)

#### File: data\_FeederVisits.csv

**Description:** This file contains each bird's visit recording to the feeders from January 9 to February 28, 2023 (inclusive), but excludes February 15 to February 23, 2023 (inclusive).

##### Variables

* VisitDate: date of observation (YYYY-MM-DD)
* Time: time of visit
* Feeder: location of feeder visited (02A, 04A, 09A, 11A, 12A, 16A)
* TransponderHexCode: unique 10-digit hexadecimal PIT tag code
* UniqueFeederCount_Total: the number of unique feeders visited by the bird calculated across the entire study period
* UniqueFeederCount_Day: the number of unique feeders visited by the bird on the given VisitDate

## Code/software

All analyses were conducted using R statistical software v. 4.3.3 using the R Studio interface. The complete code is provided in the file called:

#### File: BCCHSpatialBehav\_Script.R

**Description:** This file contains code to reproduce all main text and supplementary analyses. All packages required to run the code and reproduce analyses and figures are provided within the R code, including version numbers.

## Access information

Other publicly accessible locations of the data:

* Code and data are also available on Open Science Framework (osf.io/7hnfk)

