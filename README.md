# Streetspace dataset London

This page describes the technical specifications and brief summary of the streetspace dateset of London. The data is presented as geometric linear features representing the road centre line of streets.

<img src="sample.png" width="400">

## Methodolgy

The dataset is generated through a processing model using QGIS and R softwares. Metrics of pavement and carriageway widths are derived from urban topographic data published for research puposes by Ordnance Survey (OS) under a Digimap Licence. The full methodology is presented in the CASA Working Paper 212 ["Quantifying and Mapping Streetspace: a Geocomputational Method for the Citywide Analysis of Pedestrian and Vehicular Streetspace"](https://www.ucl.ac.uk/bartlett/casa/publications/2019/sep/casa-working-paper-212) by Nicolas Palominos and Duncan A Smith published September 2019.

## Codebook

| Variable name | Variable description |
|----|----|
|id | Unique identifier |
|DISTNAME | Street name |
|ROADNUMBER | Street code |
|CLASSIFICA | Street classification (see [OS Road type](https://www.ordnancesurvey.co.uk/xml/codelists/map/RoadClassificationTypeOML.xml) codelist)|
|foW | Aggregated footway width (both pavements added) see methodology for details |
|caW | Carriageway widths |
|toW | Total street widths |

## Format

The dataset is provided in a geopackage format (gpkg).

Data can be analysed using the free software environment R with the [sf](https://cran.r-project.org/web/packages/sf/index.html) package or the free and open-source software [QGIS](https://qgis.org/en/site/)

## Caveats

The parameters presented in this dataset should be viewed as estimated measurements of real-world-objects. For a full assessment of the data generation process read the referenced [paper](https://www.ucl.ac.uk/bartlett/casa/publications/2019/sep/casa-working-paper-212). Some known limitations are present in the measurments of bridges structures and motorways junctions were streetspace designations could be over and underestimated.

## Study area

The dataset describes all streets within an area of 2 km buffer from the M25 orbital motorway road centreline.

## Related research

This dataset was created by [Nicolas Palominos](https://npalomin.github.io/) for research purposes during the development of his PhD thesis at the Centre for Advanced Spatial Analysis. The thesis is under the supervision of Dr Duncan A Smith and Dr Sam Griffiths.

|Research Publication| Type | |
|--|--|--|
|Citywide analysis of streetspace in London |[Conference presentation](https://www.researchgate.net/publication/337745659_Citywide_analysis_of_streetspace_in_London?channel=doi&linkId=5de83ad9299bf10bc34049c8&showFulltext=true#fullTextFileContent) |3rd INTERNATIONAL LAND USE SYMPOSIUM. Land use changes: Trends and projections |
|Streetspace designation metrics |[Poster presentation](https://drive.google.com/file/d/1RwEJdtj4UGNIczO6PAgMO89gK3Xps9Qn/view) |London Walking and Cycling conference 2019 |
