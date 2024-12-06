# RSA_Data_RC

At the moment the following files are available:

## rsa_rsr_public.csv
This file has one row for each RSA (Rehabilitation Service Area) and the following columns:
* **RSA**: The Rehabilitation Service Area
* **RSA_Name**: The human-readable descriptive unique name of each RSA
* **Community_Discharge**: Successful community discharge rate for each RSA
* **CMS_region**: [The CMS region](https://www.cms.gov/about-cms/where-we-are/regional-offices) to which this RSA belongs
* **CMS_office**: [The city in which this CMS regional office is located](https://www.cms.gov/about-cms/where-we-are/regional-offices)

## rsa_xwalk_public.csv
This file has one row for each available combination of ZCTA and RSA (Rehabilitation Service Area) so that you can map various datasets indexed by ZCTA onto RSAs. Each RSA has many ZCTAs so the RSA-specific data is repeated (i.e. left-joined from rsa_rsr_public.csv, above). This file has the following columns:
* **RSA**: The Rehabilitation Service Area
* **ZCTA**: The ZIP code tabulation area
* **RSA_Name**: The human-readable descriptive unique name of each RSA
* **CMS_region**: [The CMS region](https://www.cms.gov/about-cms/where-we-are/regional-offices) to which this RSA belongs
* **CMS_office**: [The city in which this CMS regional office is located](https://www.cms.gov/about-cms/where-we-are/regional-offices)

Please cite the following DOI if you are using this data: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.13983385.svg)](https://doi.org/10.5281/zenodo.13983385)
