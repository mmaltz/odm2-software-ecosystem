# Welcome to the ODM2 Organization
This is a meta-repository to help navigate the many repositories under the [ODM2 GitHub Organization](https://github.com/ODM2).

ODM2 is both an information model and a supporting software ecosystem. The ODM2 development team is a group of researchers working across geoscience disciplines to develop and implement the ODM2 information model and supporting software tools for collecting, storing, managing, and sharing feature-based Earth Observations in a way that extends interoperability, improves data sharing, and supports scientific research. 

* View primary [documentation](https://github.com/ODM2/ODM2/wiki/documentation) for the ODM2 Information Model* 

# ODM2 GitHub Repositories and Software Ecosystem
The following are all active development repositories for different tools related to ODM2.

**ODM2 Blank RDBMS Schemas**: SQL Scripts for generating blank ODM2 databases
* Support for multiple RDBMS
    * MS SQL Server
    * MySQL
    * PostgreSQL
    * SQLite
* SQL scripts to create blank instances of ODM2 databases
* SQL script(s) to convert ODM 1.1.1 databases to ODM2 databases
* [Python script to automatically load CV terms](https://github.com/ODM2/ODM2/tree/master/src/load_cvs) from the master lists at http://vocabulary.odm2.org into a blank instance of an ODM2 database.
* [https://github.com/ODM2/ODM2](https://github.com/ODM2/ODM2) 

**ODM2 Controlled Vocabularies**:  A Python/Django-based web application for managing the ODM2 controlled vocabularies
* Online submittal and moderation of new terms and changes to existing terms
* Views of all existing vocabularies and terms
* REST-based web services exposing the vocabularies using SKOS
* Application deployed at [http://vocabulary.odm2.org](http://vocabulary.odm2.org)
* [https://github.com/ODM2/ODM2ControlledVocabularies](https://github.com/ODM2/ODM2ControlledVocabularies)

**ODM2 Python API**: A Python API for ODM2 developers
* SQL Alchemy based
* Cross platform compatible
* Interaction with an ODM2 database instance via Python
* Supports objects and methods for ODM2
* [https://github.com/ODM2/ODM2PythonAPI](https://github.com/ODM2/ODM2PythonAPI) 

**ODM Tools Python**: A Python-based desktop application for visualization, management, and quality control of environmental time series data stored in an ODM database
* Releases are available for ODM 1.1.1 and ODM2
* Based on the ODM2 Python API
* Cross platform compatible
* Time series selection and plotting
* Summary statistics
* Data export to text
* Automated Python scripting of time series quality control
* [https://github.com/ODM2/ODMToolsPython](https://github.com/ODM2/ODMToolsPython) 

**ODM2 YAML Observations Data Archive (YODA) Format and Excel Templates**:  A text-based data exchange format for ODM2 Datasets based on YAML and Microsoft Excel data templates for preparing data to be loaded into an ODM2 database instance.
* Multiple profiles for ODM2 Result types, 
    * Time series
    * Specimen time series
    * Specimen datasets
* Excel based template(s) for data entry and then export as YODA files or import to and ODM2 database using the ODM2 Data Loader
* [https://github.com/ODM2/YODA-File](https://github.com/ODM2/YODA-File) 

**ODM2 Data Loader**:  A Python-based desktop program for opening a YODA file or correctly formatted Microsoft Excel template and loading it into an ODM2 database.  Also enables export of Excel template or YODA files.
* Based on the ODM2 Python API
* Opens YODA files, parses, validates, and then loads dataset to an ODM2 database
* Opens Excel template files, parses, validates, and then loads dataset to an ODM2 database
* Provides tools for converting between Excel templates and YODA files
* Cross platform compatible
* [https://github.com/ODM2/YODA-Tools](https://github.com/ODM2/YODA-Tools) 

**ODM2 Streaming Data Loader**: A Python-based desktop application for loading table-based datalogger files into an ODM2 database.
* Based on the ODM2 Python API
* Cross platform and cross database compatible (i.e., MSSQL, MySQL, PostgreSQL, SQLite)
* Consists of a GUI for configuration and an executable for scheduled execution
* Can be scheduled to automate data loading process for sensor data into an ODM2 database
* [https://github.com/ODM2/ODM2StreamingDataLoader](https://github.com/ODM2/ODM2StreamingDataLoader) 

**ODM2 Equipment Management**:  A Python/Django-based web application for managing field monitoring equipment
* Manages metadata about site locations, site visits, field activities, instrument deployments/retrievals, calibrations, etc.
* Uses the ODM2 Equipment extension
* [https://github.com/UCHIC/ODM2Sensor](https://github.com/UCHIC/ODM2Sensor) 

**WaterOneFlow for ODM2**:  A Python web service for publishing time series observations stored in an ODM2 database using standard CUAHSI WaterOneFlow interface and WaterML XML encoding.
* Based on WOFPy
* Currently limited to time series Results from ODM2
* [https://github.com/ODM2/WOFpy](https://github.com/ODM2/WOFpy) 

**ODM2 RESTful Web Services**: A RESTful web service interface for delivering data from an ODM2 database
* More extensive than WaterOneFlow
* Capable of delivering multiple data/result types (not limited to time series)
* [https://github.com/ODM2/ODM2RESTfulWebServices](https://github.com/ODM2/ODM2RESTfulWebServices) 

**Time Series Analyst**:  A Python/Django-based web application for visualizing environmental time series data.
* Retrieves data from a WaterOneFlow web service
* Uses a simple catalog service built when the application is deployed
* Visualizations developed using D3.js
* [https://github.com/UCHIC/WEBTSA](https://github.com/UCHIC/WEBTSA) 

**HydroShare ODM2 Time Series**: An implementation of ODM2 in SQLite for storing hydrologic time series in HydroShare
* Online import of time series as either an ODM2 SQLite database or simple CSV table
* Online editing of ODM2/HydroShare metadata and syncing with the underlying SQLite database
* Export of an ODM2 compliant SQLite database
* Deployed in HydroShare at https://www.hydroshare.org
* [https://github.com/hydroshare/hydroshare](https://github.com/hydroshare/hydroshare) 

**ODM2 Web Streaming Data Loader**: A Python/Django-based web application and web service for registering data collection devices and allowing them to stream sensor observations into an online instance of an ODM2 database.
* Enabling citizen science with Stroud Water Research Center and Enviro DIY Arduino dataloggers
* Implements simple REST web service for devices to POST data to the service and have it stored in an ODM2 database instance as the backend
* Implements a front end website for users to register sites/data collection devices, list the observed variables, and create the metadata needed to enable data streaming.
* Currently deployed at http://data.envirodiy.org
* [https://github.com/ODM2/ODM2WebSDL](https://github.com/ODM2/ODM2WebSDL)

**ODM2 Admin**: A web-based Django/Python admin app for an ODM2 database instance. 
* Provides data input capabilities
* Includes simple data visualizations for time series and environmental specimens
* Functionality for managing data derived from environmental specimens
* [https://github.com/ODM2/ODM2-Admin](https://github.com/ODM2/ODM2-Admin)

# Support and Credits
ODM2 and related software have been developed under funding from several different sources. This work was supported by National Science Foundation Grants [EAR-1224638](http://www.nsf.gov/awardsearch/showAward?AWD_ID=1224638), [ACI-1339834](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1339834)). Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation. 

ODM2 draws heavily from our prior work with the CUAHSI Hydrologic information system and ODM 1.1.1 (Horsburgh et al., 2008; Horsburgh and Tarboton, 2008), our experiences working on the Critical Zone Observatory Integrated Data Management System (CZOData), and our experiences with the EarthChem systems (e.g., Lehnert et al., 2007; 2009). It also extensively uses concepts from the Open Geospatial Consortium's Observations & Measurements standard (Cox, 2007a; 2007b; 2011a; 2011b; ISO, 2011).

# References
[See a full list of ODM2 related references](https://github.com/ODM2/ODM2/wiki/References)
