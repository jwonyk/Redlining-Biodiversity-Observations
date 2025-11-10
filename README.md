# HOLC Redlining and Biodiversity Observations

## Purpose of this project

This project explores how historical redlining practices, a discriminatory neighborhood grading by Home Owner's Loan Corporation (HOLC) in the 1930s, which continued to linger and caused environmental and ecological conditions in Los Angeles today. We also have GBIF bird observation records to see the effects of socioeconomic and environmental factors. The goal is to show the legacy of structural discrimination in urban planning, even til today, using three elements:

-   Air Quality

-   Long-Term Health Outcome

-   Low Income

## Repository Structure

``` bash
.
├── data
│   ├── ejscreen
│   │   ├── EJSCREEN_2023_BG_StatePct_with_AS_CNMI_GU_VI.gdb
│   │   ├── EJSCREEN_LA.gpkg
│   ├── gbif-birds-LA
│   │   ├── gbif-birds-LA.dbf
│   │   ├── gbif-birds-LA.prj
│   │   ├── gbif-birds-LA.shp
│   │   └── gbif-birds-LA.shx
│   └── mapping-inequality
│       └── mapping-inequality-los-angeles.json
├── EDS223-HW2.Rproj
├── HW2.html
├── HW2.qmd
└── README.md
```

## Data Access

This project uses publicly available spatial data sets that are loaded using the R `sf` package. All data required to reproduce the analysis are stored locally within the project repository in the `data/` directory.

The first dataset is the **EJScreen** data from the [U.S. Environmental Protection Agency](https://www.epa.gov/)’s Environmental Justice Screening and Mapping Tool. Although the tool is no longer active, the data were publicly available [here](https://pedp-ejscreen.azurewebsites.net/) and have been archived locally in the project repository. The data set provides environmental and demographic indicators at the Census block group level across the United States.

The second data set is the **Mapping Inequality Project** redlining data, developed by the [Digital Scholarship Lab](https://dsl.richmond.edu/) at the University of Richmond. These data digitize historical Home Owners’ Loan Corporation (HOLC) maps and classifications for U.S. cities. For this project, we use the Los Angeles subset, which includes spatial polygons of HOLC grade designations. The full collection is available through the project [website](https://dsl.richmond.edu/panorama/redlining/data).

The third data set is **bird observation** data from the Global Biodiversity Information Facility (GBIF), accessed for records in the Los Angeles region from 2021 onward. The data are stored locally as a shapefile and include georeferenced species observations with associated metadata. Information of following data can be found [here](https://www.gbif.org/dataset/4fa7b334-ce0d-4e88-aaae-2e0c138d049e).

## Authorship

-   The project author: **Jay Kim**
-   Instructor: **Annie Adams**
-   Teaching Assistant: **Ale Vidal Meza**

## Reference

Gee, G. C. (2008). A multilevel analysis of the relationship between institutional and individual racial discrimination and health status. American journal of public health, 98(Supplement_1), S48-S56.

Nardone, A., Rudolph, K. E., Morello-Frosch, R., & Casey, J. A. (2021). Redlines and greenspace: the relationship between historical redlining and 2010 greenspace across the United States. Environmental health perspectives, 129(1), 017006.

Hoffman, J. S., Shandas, V., & Pendleton, N. (2020). The effects of historical housing policies on resident exposure to intra-urban heat: a study of 108 US urban areas. Climate, 8(1), 12.

Ellis-Soto, D., Chapman, M., & Locke, D. H. (2023). Historical redlining is associated with increasing geographical disparities in bird biodiversity sampling in the United States. Nature Human Behaviour, 1-9.

Robert K. Nelson, LaDale Winling, Richard Marciano, Nathan Connolly, et al., “Mapping Inequality,” American Panorama, ed. Robert K. Nelson and Edward L. Ayers, accessed October 17, 2023, <https://dsl.richmond.edu/panorama/redlining/>

United States Environmental Protection Agency. 2015. EJSCREEN. Retrieved: October 17th, 2025, www.epa.gov/ejscreen.
