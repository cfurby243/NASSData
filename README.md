# NASS DATA 2002 - 2015

Provided is the open source data provided by The National Automobile Sampling System (NASS) converted to a CVS file instead of the original 
SAS file.

The [The datasets](ftp://ftp.nhtsa.dot.gov/nass )  used in the new analyses are available to the public on the [NHTSA website](https://www.nhtsa.gov/research-data/national-automotive-sampling-system-nass). All of the information about how to access the data, as well as the SAS code used to merge and concatenate data sets, can be found within the R code and below. Comments have been made indicting what has been done and what each code line does.

The documentation for the data sets can be downloaded from the same site. The four SAS data sets used are as follows;

**"Occupant Assessment"** - Providing information about the occupant and injuries

**"General Vehicle"** - Providing information about the impact speeds and the vehicle model

**"Vehicle Exterior"** -  Provides the direction of impact

**"Accident Description"** -  Provides the "ratio inflation factor" used for weighting the data. 

These data sets are provided for each year. Individual cases are distinguished by year of accident, primary sampling unit, and case ID. The case IDs refer to the accident; within accident individual cars are identified by a "vehicle number" and within vehicles, each occupant is identified by an "occupant number". Using these identifiers, the user may combine the data sets. 

### **Occupant Assessment**

As a reminder: Occupant Assessment provides information about the occupant and injuries squired.
Variables used from the "Occupant Assessment" data sets include;

**"AGE"** - 'AGE OF OCCUPANT'

**"BAGAVAIL"** - 'AIR BAG SYSTEM AVAILABILITY'

**"BAGDEPLY"** - 'AIR BAG SYSTEM DEPLOYED'

**"BAGFAIL"** - 'AIR BAG SYSTEM FAILURE'

**"CASEID"** - 'CASE NUMBER - STRATUM'

**"CASENO"** - 'CASE SEQUENCE NUMBER'

**"CHTYPE"** - 'TYPE OF CHILD SAFETY SEAT'

**"DEATH"** - 'TIME TO DEATH'

**"HEIGHT"**  - 'HEIGHT OF OCCUPANT'

**"HOSPSTAY"** - 'HOSPITAL STAY'

**"INJSEV"**   - 'INJURY SEVERITY (POLICE RATING)'

**"MANUSE"**  - 'MANUAL BELT SYSTEM USE'

**"OCCNO"**  - 'OCCUPANT NUMBER'

**"PSU"**  - 'PRIMARY SAMPLING UNIT NUMBER'

**"ROLE"**  - 'OCCUPANT'S ROLE'

**"SEATPOS"** - 'OCCUPANT'S SEAT POSITION'

**"SEX"**   - 'OCCUPANT'S SEX'

**"TREATMNT"** - 'TREATMENT - MORTALITY'

**"VEHNO"**  -  'VEHICLE NUMBER'

**"WEIGHT"**  -  'OCCUPANT'S WEIGHT'

As a reminder: the "general vehicle" file, provided information about the impact speeds and the vehicle model. 
The variables used to create data set for General Vehicle data include;

**"PSU"** - 'PRIMARY SAMPLING UNIT NUMBER'

**"CASEID"** - 'CASE NUMBER - STRATUM'

**"VEHNO"** - 'VEHICLE NUMBER'

**"BODYTYPE"** - 'VEHICLE BODY TYPE'

**"MODELYR"** - 'VEHICLE MODEL YEAR'

**"DVTOTAL"** - 'TOTAL DELTA V'

**"DVBASIS"** - 'BASIS FOR TOTAL DELTA V (HIGHEST)'

**"DVEST"** - 'ESTIMATED HIGHEST DELTA V'

**"MAKE"** - 'VEHICLE MAKE'

### **"Vehicle Exterior"**

As a reminder: the "Vehicle Exterior" data provides the direction of impact.

The variables used to create this data table include; 

**"PSU"** - 'PRIMARY SAMPLING UNIT NUMBER'

**"DOF1"** - 'DIRECTION OF FORCE (HIGHEST)'

**"CASEID"** -'CASE NUMBER - STRATUM'

**"GAD1"** - 'DEFORMATION LOCATION (HIGHEST)'

### **"Accident Description"**

As a reminder: The "Accident Description" data table provides the "ratio inflation factor" used for weighting the data. 

The variables used to create the data table were;

**"PSU"** - 'PRIMARY SAMPLING UNIT NUMBER'

**"STRATIF"** - 'CASE STRATUM'

**"CASEID"** - 'CASE NUMBER - STRATUM'
