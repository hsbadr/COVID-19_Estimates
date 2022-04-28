# COVID-19_Estimates

[![Copyright: © 2022 JHU)](https://img.shields.io/badge/Copyright-%C2%A9%202022%20JHU-blue.svg)](https://systems.jhu.edu)
[![Credits: NASA/NIH](https://img.shields.io/badge/Credits-NASA%20&%20NIH-blue.svg)](#Credits)
[![DOI: 10.1101/2021.05.05.21256712](https://zenodo.org/badge/DOI/10.1101%2F2021.05.05.21256712.svg)](https://doi.org/10.1101/2021.05.05.21256712)
[![GitHub Commit](https://img.shields.io/github/last-commit/CSSEGISandData/COVID-19_Unified-Dataset)](https://github.com/CSSEGISandData/COVID-19_Unified-Dataset/commits/master)

This is a part of the [unified COVID-19 dataset](https://github.com/CSSEGISandData/COVID-19_Unified-Dataset) to provide epidemiological estimates of infections and effective reproduction number.

The estimates are generated using [`EpiNow2`](https://cran.r-project.org/package=EpiNow2) and [`EpiEstim`](https://cran.r-project.org/package=EpiEstim) R packages. The parameters required for Rt estimates, specifically the distributions of incubation period and serial interval, are obtained from the literature.

## COVID-19 Estimates Data Structure

|    Column     |   Type    | Description                                                  |
| :-----------: | :-------: | :------------------------------------------------------------|
|    **ID**     | Character | Geospatial ID, unique identifier                             |
|   **Date**    |   Date    | Date of data record                                          |
|    **I**      |  Double   | Estimates of daily infections                                |
|    **R**      |  Double   | Estimates of effective reproduction number                   |
|   **Type**    | Character | Type of the estimated infections                             |
|    **Age**    | Character | Age group of the estimated infections                        |
|    **Sex**    | Character | Sex/gender of the estimated infections                       |
|  **Source**   | Character | Epidemiological data source as listed in the unified dataset |

## Credits

This work is supported by NASA Health & Air Quality project `80NSSC18K0327`, under a COVID-19 supplement, and National Institute of Health (NIH) project `3U19AI135995-03S1` ("Consortium for Viral Systems Biology (CViSB)"; Collaboration with The Scripps Research Institute and UCLA).

## Citation

To cite this dataset:

> Badr, H. S., B. F. Zaitchik, G. H. Kerr, N. Nguyen, Y. Chen, P. Hinson, J. M. Colston, M. N. Kosek, E. Dong, H. Du, M. Marshall, K. Nixon, A. Mohegh, D. L. Goldberg, S. C. Anenberg, and L. M. Gardner, **2021**: Unified real-time environmental-epidemiological data for multiscale modeling of the COVID-19 pandemic. *MedRxiv*, 2021.05.05.21256712.

### BibTeX

```latex
@article {Badr2021.05.05.21256712,
	author = {Badr, Hamada S. and Zaitchik, Benjamin F. and Kerr, Gaige H. and Nguyen, Nhat-Lan and Chen, Yen-Ting and Hinson, Patrick and Colston, Josh M. and Kosek, Margaret N. and Dong, Ensheng and Du, Hongru and Marshall, Maximilian and Nixon, Kristen and Mohegh, Arash and Goldberg, Daniel L. and Anenberg, Susan C. and Gardner, Lauren M.},
	title = {Unified real-time environmental-epidemiological data for multiscale modeling of the COVID-19 pandemic},
	elocation-id = {2021.05.05.21256712},
	year = {2021},
	doi = {10.1101/2021.05.05.21256712},
	publisher = {Cold Spring Harbor Laboratory Press},
	abstract = {An impressive number of COVID-19 data catalogs exist. None, however, are optimized for data science applications, e.g., inconsistent naming and data conventions, uneven quality control, and lack of alignment between disease data and potential predictors pose barriers to robust modeling and analysis. To address this gap, we generated a unified dataset that integrates and implements quality checks of the data from numerous leading sources of COVID-19 epidemiological and environmental data. We use a globally consistent hierarchy of administrative units to facilitate analysis within and across countries. The dataset applies this unified hierarchy to align COVID-19 case data with a number of other data types relevant to understanding and predicting COVID-19 risk, including hydrometeorological data, air quality, information on COVID-19 control policies, and key demographic characteristics.Competing Interest StatementThe authors have declared no competing interest.Funding StatementThis work is supported by NASA Health \&amp; Air Quality project 80NSSC18K0327, under a COVID-19 supplement, National Institute of Health (NIH) project 3U19AI135995-03S1 ("Consortium for Viral Systems Biology (CViSB)"; Collaboration with The Scripps Research Institute and UCLA), and NASA grant 80NSSC20K1122. Johns Hopkins Applied Physics Laboratory (APL), Data Services and Esri provide professional support on designing the automatic data collection structure, and maintaining the JHU CSSE GitHub repository.Author DeclarationsI confirm all relevant ethical guidelines have been followed, and any necessary IRB and/or ethics committee approvals have been obtained.YesThe details of the IRB/oversight body that provided approval or exemption for the research described are given below:IRB approval is not required.All necessary patient/participant consent has been obtained and the appropriate institutional forms have been archived.YesI understand that all clinical trials and any other prospective interventional studies must be registered with an ICMJE-approved registry, such as ClinicalTrials.gov. I confirm that any such study reported in the manuscript has been registered and the trial registration ID is provided (note: if posting a prospective study registered retrospectively, please provide a statement in the trial ID field explaining why the study was not registered in advance).Yes I have followed all appropriate research reporting guidelines and uploaded the relevant EQUATOR Network research reporting checklist(s) and other pertinent material as supplementary files, if applicable.YesThe source code used to clean, unify, aggregate, and merge the different data components from all sources will be available on GitHub.https://github.com/CSSEGISandData/COVID-19_Unified-Dataset},
	URL = {https://www.medrxiv.org/content/early/2021/05/07/2021.05.05.21256712},
	eprint = {https://www.medrxiv.org/content/early/2021/05/07/2021.05.05.21256712.full.pdf},
	journal = {medRxiv}
}
```
