**Disclaimer:**
  The current Python model codes are in an Alpha state. Further work is intended to improve detection capability and improve functionality of the model. The files provided are the raw python code to set up the tools. Setup of the tools is still required (see Setup of Tools for instructions). If any bugs are found, please report them.

**Program required to run file:**
   - ArcGIS Pro or ArcGIS Online

**Files Required to Run:**
  - Crater Slope Detection Model: A Digital Terrain Model (DTM) or Digital Elevation Model (DEM) of the region.
  - Diameter-Depth Calculator: A Digital Terrain Model (DTM) or Digital Elevation Model (DEM) of the region and a polygon file of your identified craters.
  - External Slope & Internal Basin: Raster data file you wish to examine (such as geochemical) and a polygon file of your identified craters.

**Files Recommended:**
  - Photo-Imagery of the region you wish to investigate.

**Pre-Model Prep:**
  - We recommend creating a polygon clip file of the region you intend to investigate for your DTM/DEM. This will improve program speed and later clean up of detected features.

---

**Setup of Tools**
To install these tools, you will need to create a new Script in your toolbox. Copy the code into the Execution Tab, and then in Parameters, set up the following:

Crater Slope Detection Model:

Parameter 0:

    Label: Input DTM/DEM
    Data Type: Raster Dataset
    Direction: Input
    Type: Required

Parameter 1:

    Label: Upper Threshold
    Data Type: Double (or Long if it's an integer)
    Direction: Input
    Type: Required

Parameter 2:

    Label: Lower Threshold
    Data Type: Double (or Long if it's an integer)
    Direction: Input
    Type: Required

Parameter 3:

    Label: Output Workspace
    Data Type: Workspace
    Direction: Input
    Type: Required

Parameter 4:

    Label: Output Polygon Features
    Data Type: Feature Class
    Direction: Output
    Type: Derived (since this is the result of the script, not something the user inputs directly). 

Diameter-Depth Calculator

Parameter 0:

    Label: Input DTM/DEM
    Data Type: Raster Dataset
    Direction: Input
    Type: Required

Parameter 1:

    Label: Upper Threshold
    Data Type: Double (or Long if it's an integer)
    Direction: Input
    Type: Required

Parameter 2:

    Label: Lower Threshold
    Data Type: Double (or Long if it's an integer)
    Direction: Input
    Type: Required

Parameter 3:

    Label: Output Workspace
    Data Type: Workspace
    Direction: Input
    Type: Required

Parameter 4:

    Label: Output Polygon Features
    Data Type: Feature Class
    Direction: Output
    Type: Derived (since this is the result of the script, not something the user inputs directly). 

External Slope and Internal Basin

Parameter 0:

    Label: Input DTM/DEM
    Data Type: Raster Dataset
    Direction: Input
    Type: Required

Parameter 1:

    Label: Upper Threshold
    Data Type: Double (or Long if it's an integer)
    Direction: Input
    Type: Required

Parameter 2:

    Label: Lower Threshold
    Data Type: Double (or Long if it's an integer)
    Direction: Input
    Type: Required

Parameter 3:

    Label: Output Workspace
    Data Type: Workspace
    Direction: Input
    Type: Required

Parameter 4:

    Label: Output Polygon Features
    Data Type: Feature Class
    Direction: Output
    Type: Derived (since this is the result of the script, not something the user inputs directly). 
