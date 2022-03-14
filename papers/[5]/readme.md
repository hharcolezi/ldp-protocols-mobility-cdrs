## Title
Preserving Geo-Indistinguishability of the Emergency Scene to Predict Ambulance Response Time

## Abstract
Emergency medical services (EMS) provide crucial emergency assistance and ambulatory services. One key measurement of EMS’s quality of service is their ambulances’ response time (ART), which generally refers to the period between EMS notification and the moment an ambulance arrives on the scene. Due to many victims requiring care within adequate time (e.g., cardiac arrest), improving ARTs is vital. This paper proposes to predict ARTs using machine-learning (ML) techniques, which could be used as a decision-support system by EMS to allow a dynamic selection of ambulance dispatch centers. However, one well-known predictor of ART is the location of the emergency (e.g., if it is urban or rural areas), which is sensitive data because it can reveal who received care and for which reason. Thus, we considered the ‘input perturbation’ setting in the privacy-preserving ML literature, which allows EMS to sanitize each location data independently and, hence, ML models are trained only with sanitized data. In this paper, geo-indistinguishability was applied to sanitize each emergency location data, which is a state-of-the-art formal notion based on differential privacy. To validate our proposals, we used retrospective data of an EMS in France, namely Departmental Fire and Rescue Service of Doubs, and publicly available data (e.g., weather and traffic data). As shown in the results, the sanitization of location data and the perturbation of its associated features (e.g., city, distance) had no considerable impact on predicting ARTs. With these findings, EMSs may prefer using and/or sharing sanitized datasets to avoid possible data leakages, membership inference attacks, or data reconstructions, for example.

## Experiments
* Please refer to [1_Geo_Indistinguishability.ipynb](https://github.com/hharcolezi/ldp-protocols-mobility-cdrs/blob/main/papers/%5B5%5D/1_Geo_Indistinguishability.ipynb) for the code of a Laplace mechanism that satisfy geo-indistinguishability.

## Recommended citation
Arcolezi, H.H.; Cerna, S.; Guyeux, C.; Couchot, J.-F. Preserving Geo-Indistinguishability of the Emergency Scene to Predict Ambulance Response Time. Math. Comput. Appl. 2021, 26, 56. https://doi.org/10.3390/mca26030056.

## Bibtex
@article{Arcolezi2021,
author = {Arcolezi, Héber H. and Cerna, Selene and Guyeux, Christophe and Couchot, Jean-François},
title = {Preserving Geo-Indistinguishability of the Emergency Scene to Predict Ambulance Response Time},
journal = {Mathematical and Computational Applications},
volume = {26},
year = {2021},
number = {3},
pages = {56},
issn = {2297-8747},
doi = {10.3390/mca26030056}
}

