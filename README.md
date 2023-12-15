# Aphasia Recovery Cohort (ARC) Dataset

## Overview

This dataset includes anonymized images, behavioral measures and demographic details from a cohort of individuals with chronic stroke as well as speech and language impairments. This meta-dataset combines imaging data from multiple independent studies conducted in South Carolina, with many individual's participating in multiple sessions both within studies and across studies. This aspect enables longitudinal research. The dataset also includes multiple modalities, including anatomical (T1w, T2w, FLAIR), functional (fMRI), resting-state and diffusion protocols (albeit sequences evolved across studies, as described in the BIDS format sidecar files). Further, the dataset is fully anonymized, allowing public sharing which is vital for education. These unique features complement existing repositories of [acute](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10444746/ and [chronic](https://pubmed.ncbi.nlm.nih.gov/32310331/) stroke.

## Data Contents
* `participants.tsv` - List of subject IDs, demographic variables, and impairment measures. Note that many variables are [generalized](https://www.hhs.gov/hipaa/for-professionals/privacy/special-topics/de-identification/index.html#approachmitigate) to meet [International Safe Harbor Privacy Principles](https://en.wikipedia.org/wiki/International_Safe_Harbor_Privacy_Principles).


* `Subject Directories` - MRI data directories for each subject. Each session is named based on the days post stroke for the scanning session (e.g. `ses-520` was acquired 520 days post-injury):
  - `anat` - T1 anatomical images
  - `dwi` - Diffusion weighted images
  - `fmap` - Magnitude and phase difference fieldmap images
  - `func` - [Naming](https://onlinelibrary.wiley.com/doi/full/10.1002/hbm.20683) task and resting state data

