# Entwicklung einer FOSSGIS-basierten Analyse zur Unterstützung von Such- und Rettungsaktionen

## Description

The objective of this project is to develop a QGIS-Workflow (built in the Graphical Modeler) to support search and rescue operations, resulting in a cost distance surface. This indicates the maximum distance the person can move in a given time.

The workflow includes different factors in the analysis, such as the topography, the road infrastructure or the prevailing vegetation. The theoretical basis here is the calculation of a cost surface, which is represented as a final product in a cumulative cost distance surface. Different costs are assigned to the input parameters (CORINE data, OSM data, DEM) and integrated into a variable cost surface on which human mobility behavior can be modeled under the assumption of cost minimization. This allowed to represent maximum spatial distances that can be traveled within certain time intervals. This was tested in two different study areas, on the one hand in Mühlhausen in Kraichgau and on the other hand in the province of Vorarlberg in Austria.

## Getting Started

* The entire workflow is based on a model using QGIS. The work was done using the current stable QGIS Version 3.28.4 (https://www.qgis.org/de/site/forusers/download.html). A download of this program is necessary to run the developed analysis.
* Furthermore the following QGIS-Plugin should be installed: SRTM-Downloader

### Dependencies

* One needs to create an OpenStreetMap Account at the following website: (https://export.hotosm.org/en/v3/). This is necessary to directly download the data.
* One needs to create an NASA Earthdata Account to use the QGIS-Plugin SRTM-Downloader and direcly import the DEMs into your project. This can be found under the following link: https://urs.earthdata.nasa.gov//users/new
* One needs to create an Account at the Copernicus Programm at the following website: https://land.copernicus.eu/pan-european/corine-land-cover/clc2018?tab=download. This is necessary to download the CORINE Land Cover (CLC) Data.
* The CORINE data is not provided through the heiBOX because of the size of the dataset.

### Data download

* The provided scripts for filtering the needed OSM data using the ohsome API (optional) and the ORS comparison can be copied into the appropriate field. One can run the scripts using jupyter notebook running within a suitable environment.
* To download the needed data using the HOT Export Tool one can use the provided YAML code and enter it into the Data section of the Website.

### Running the model and scripts

* All the data except CORINE are provided in the following heiBOX Link: https://heibox.uni-heidelberg.de/d/829ebf259ddb4a389165/
* Select the necessary input parameters to run the model.
* To run the scripts one can use Anaconda to launch jupyter notebook.

## Authors

Johannes Grünewald and Maximilian Schäfer