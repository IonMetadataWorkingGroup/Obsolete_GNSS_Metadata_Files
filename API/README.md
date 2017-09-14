ION GNSS SDR Metadata API
========
This repository contains XML schema and Applications Programming Interface (API) open source software for translating GNSS SDR Metadata XML documents.  

Click the following links for an example  XML metadata document : [Example GPS L1 C/A Metadata - XML format](https://raw.githubusercontent.com/IonMetadataWorkingGroup/API/master/design/Scenarios/SingleDataFile/L1GpsData.xml "Example L1 GPS  metadata").

## Repository Overview ##
The repository contains software development and XML schema artifacts.  Top level descriptions of the directories are as follows:
 
- **app** - API example applications
- **design**- schema related design artifacts including UML object models and metadata scenarios.   
- **doc** - Metadata specification documentation.  
- **include** - C++ API include directories.  
- **lib** - C++ library packages.  Contains source implementation and tinyxml2 submodule.
- **schema** - Metadata schema and related artifacts.
- **tools** - XSLT, hyperlinks, and other tools for processing metadata XML files.


## Building the API ##
Clone the git repository to a local working directory and follow the instructions for building the API and library using Windows or Linux.

### Windows ###
The API currently builds using Visual Studio 2008 solution.  This can be upgraded to more recent versions of Visual studio as needed.   Open the GnssMetadata.sln file in the root directory.  

This will show a solution framework comprised of applications and libraries.  Build the solution for a specified target (e.g. DEBUG x64).  Execute the TestApp, which demonstrates reading, writing, and creating metadata files using the API.

### Linux ###

To clone the repository.  open terminal window change directory to your development root and execute the following commands:

```
    git clone  --recursive git://github.com/IonMetadataWorkingGroup/API
    cd API
```
Build the libraries using CMAKE and install using the following commands. Within the API
directory.

```
    mkdir build
    cmake ..

    make

    sudo make install
```

## API Documentation ##
Ultimately, the API will be documented using oxygen or other code documentation tools.   Interim documentation can be found at [Metadata Object Model](./doc) in the doc directory.
