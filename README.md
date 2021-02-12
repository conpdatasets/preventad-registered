# PREVENT-AD Registered Dataset

### Overview

The PREVENT-AD (Pre-symptomatic Evaluation of Experimental or Novel Treatments for Alzheimer Disease) cohort is composed of cognitively healthy participants over 55 years old, at risk of developing Alzheimer Disease (AD) as their parents and/or siblings were/are affected by the disease. These ‘at-risk’ participants have been followed for a naturalistic study of the presymptomatic phase of AD since 2011 using multimodal measurements of various disease indicators. One clinical trial intended to test a pharmaco-preventive agent has also been conducted.

This PREVENT-AD dataset is available to researchers around the world with the intention to contribute to the community’s growing understanding of AD pathogenesis.

More detailed information about the study design can be found in the LORIS instance of Registered PREVENT-AD (https://registeredpreventad.loris.ca).

### Data organization

A `DATS.json` is present at the root of the dataset and describes the content of the dataset.

The dataset is organized in three different parts:
  
  - `clinical-data`: clinical data spreadsheets and data dictionary
  - `images-in-BIDS`: images orgnized according to the BIDS standard in the `BIDS_dataset` directory. Specifications of the BIDS standard are available [here](https://bids-specification.readthedocs.io/en/stable/).
  - `images-in-MINC`: images provided in MINC format. In this portion of the dataset, `candidate.json` contains demographic information regarding the candidate in question; `visit.json` contains visit level information, `handedness.json` when present, contains results of the Handedness Edinburgh Inventory
		
Note: the two images folders contain the same modalities and number of subjects/visits. 

```
preventad-registered
|__DATS.json
|__README.md
|__clinical-data
   |__AD8_Registered_PREVENTAD.csv
   |__APS_Registered_PREVENTAD.csv
   |__Auditory_processing_Registered_PREVENTAD.csv
   |__BP_Pulse_Weight_Registered_PREVENTAD.csv
   |__CSF_proteins_Registered_PREVENTAD.csv
   |__Data_Dictionary_Registered_PREVENTAD.csv
   |__Demographics_Registered_PREVENTAD.csv
   |__EL_CAIDE_Registered_PREVENTAD.csv
   |__EL_CDR_MoCA_Registered_PREVENTAD.csv
   |__EL_Medical_history_Registered_PREVENTAD.csv
   |__Genetics_Registered_PREVENTAD.csv
   |__Lab_Registered_PREVENTAD.csv
   |__List_of_participants_switched_back_to_cohort.txt
   |__List_of_participants_with_only_1_sibling.txt
   |__Med_categories.txt
   |__Med_use_Registered_PREVENTAD.csv
   |__RBANS_Registered_PREVENTAD.csv
   |__Smell_identification_Registered_PREVENTAD.csv
|__images-in-BIDS
   |__BIDS_dataset
      |__dataset_description.json
      |__participants.json
      |__participants.tsv
      |__README
      |__sub-<candidate_id>
         |__ses-<visit_label>
               |__sub-<candidate_id>_ses-<visit_label>_scans.json
               |__sub-<candidate_id>_ses-<visit_label>_scans.tsv
                     |__anat
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.nii.gz
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.json
                           ...
                     |__asl
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.nii.gz
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.json
                           ...
                     |__dwi
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.nii.gz
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.json
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.bval
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.bvec
                           ...
                     |__fmap
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.nii.gz
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.json
                           ...
                     |__func
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.nii.gz
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>.json
                           |__ sub-<candidate_id>_ses-<visit_label>_run-<number>_<BIDS_scan_type>_events.txt
                           ...
|__images-in-MINC
   |__candidate_id
      |__candidate.json
      |__visit_label
         |__visit.json
         |__handedness.json
         |__images
            |__image_1.mnc
            |__image_2.mnc
            |__image_3.mnc
            ...
```



### For more information: 

- LORIS registered database instance with the PREVENT-AD dataset: https://registeredpreventad.loris.ca
- PREVENT-AD study web site: https://prevent-alzheimer.net/
- PREVENT-AD Twitter account: https://twitter.com/prevent_ad
- Dataset DOI: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4298795.svg)](https://doi.org/10.5281/zenodo.4298795)



***Links to the open dataset of PREVENT-AD (basic demographics and MRIs):***

- LORIS open database instance with the PREVENT-AD dataset: https://openpreventad.loris.ca
- Open PREVENT-AD dataset: https://portal.conp.ca/dataset?id=projects/preventad-open
- Open PREVENT-AD BIDS dataset: https://portal.conp.ca/dataset?id=projects/preventad-open-bids

