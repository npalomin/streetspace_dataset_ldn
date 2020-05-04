# Streetspace dataset London

[Methodology](https://github.com/npalomin/streetspace_dataset_ldn#methodolgy)

[Codebook](https://github.com/npalomin/streetspace_dataset_ldn#codebook)

[Format](https://github.com/npalomin/streetspace_dataset_ldn#format)

[Caveats](https://github.com/npalomin/streetspace_dataset_ldn#caveats)

[Study Area](https://github.com/npalomin/streetspace_dataset_ldn#study-area)

[Licencing of OS data](https://github.com/npalomin/streetspace_dataset_ldn#licencing-of-os-data)

[Related research](https://github.com/npalomin/streetspace_dataset_ldn#related-research)

[Data accessibility](https://github.com/npalomin/streetspace_dataset_ldn#data-accessibility)

[Citation](https://github.com/npalomin/streetspace_dataset_ldn#citation)

[Contact](https://github.com/npalomin/streetspace_dataset_ldn#contact)

This page describes the technical specifications and brief summary of the streetspace dataset of London. The data is presented as geometric linear features representing the road centre line of streets.

<img src="sample.png" width="400" style="margin:0px 250px">

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

The data can be analysed using the free software environment R with the [sf](https://cran.r-project.org/web/packages/sf/index.html) package or the free and open-source software [QGIS](https://qgis.org/en/site/)

## Caveats

The parameters presented in this dataset should be viewed as estimated measurements of real-world-objects. For a full assessment of the data generation process user are adviced consider the referenced [paper](https://www.ucl.ac.uk/bartlett/casa/publications/2019/sep/casa-working-paper-212). Some known limitations are present in the measurements of bridges structures and at motorways junctions where streetspace designations could be over and underestimated. Other inconsistencies observed in the data have to do with the capacity of the datasets to synchronously reflect the ongoing changing nature of the built environment

## Study area

The dataset describes all streets within an area of 2 km buffer from the M25 Orbital Motorway road centreline.

## Licencing of OS data

Ordnance Survey has released a new [Covid-19 licence](https://www.ordnancesurvey.co.uk/about/covid-19/new-to-os) for various premium OS products free of royalties

## Related research

This dataset was created by [Nicolas Palominos](https://npalomin.github.io/) for research purposes during the development of his PhD thesis at the Centre for Advanced Spatial Analysis, University College London. The thesis is under the supervision of Dr Duncan A Smith and Dr Sam Griffiths.

|Research Publication| Type | |
|--|--|--|
|Citywide analysis of streetspace in London |[Conference presentation](https://www.researchgate.net/publication/337745659_Citywide_analysis_of_streetspace_in_London?channel=doi&linkId=5de83ad9299bf10bc34049c8&showFulltext=true#fullTextFileContent) |3rd INTERNATIONAL LAND USE SYMPOSIUM. Land use changes: Trends and projections |
|Streetspace designation metrics |[Poster presentation](https://drive.google.com/file/d/1RwEJdtj4UGNIczO6PAgMO89gK3Xps9Qn/view) |London Walking and Cycling conference 2019 |

## Data accessibility

Data are available from Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3783807.svg)](https://doi.org/10.5281/zenodo.3783807)

## Citation

Cite working paper as:

APA

Palominos, N., & Smith, D. A. Quantifying and Mapping Streetspace: a Geocomputational Method for the Citywide Analysis of Pedestrian and Vehicular Streetspace. CASA Workig Paper 212. Sep 2019.

Bibtex

@article{palominos_quantifying_2019,
    series = {{CASA} {Working} {Paper} 212},
    title = {Quantifying and {Mapping} {Streetspace}: a {Geocomputational} {Method} for the {Citywide} {Analysis} of {Pedestrian} and {Vehicular} {Streetspace}},
    issn = {1467-1298},
    url = {https://www.ucl.ac.uk/bartlett/casa/sites/bartlett/files/casa_working_paper_-_212.pdf},
    language = {en},
    author = {Palominos, Nicolas and Smith, Duncan A},
    month = sep,
    year = {2019},
    pages = {21}
}

## Contact

For enquiries contact Nicolas Palominos at n.palominos.16@ucl.ac.uk
