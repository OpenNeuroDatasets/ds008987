# Adult resting-state functional MRI derivatives
This dataset contains de-identified derivative anatomical and resting-state functional MRI images from the adult comparison sample analyzed in Jung and Dilks, "A fine-grained cortical blueprint for three scene systems in newborns".

## Participants
The published adult comparison includes 40 adults (18–39 years; 23 female). 

## Data
- `sub-*/anat/*_T1w.nii.gz`: defaced anatomical image. Check the exact `desc-` label against the processing level of the shared image.
- `sub-*/func/*_task-rest_desc-clean_bold.nii.gz`: cleaned resting-state functional image in native space (T1w).

## Processing
Resting-state EPI preprocessing included AFNI-based despiking, motion correction, nuisance regression (6 motion parameters, 6 derivatives, white-matter and ventricular signals), and temporal filtering (0.008–0.1 Hz). 
No spatial smoothing was applied. Anatomical images were defaced before public release. Details and software versions should be checked against the final manuscript and updated here where necessary.

## Acquisition
Resting-state functional scans used TR = 2.0 s (or TR = 1.5 s for some participants) and TE = 30 ms, with 2 mm isotropic voxels, as documented in the manuscript. Verify metadata against original acquisition records. Participants were scanned awake.

## Data use and privacy
All aspects of fMRI data collection was approved by the Institutional Review Board of Emory University (#69592), and written consent was obtained before the experiment.

## Associated code
https://github.com/yaelanjung/infantSceneConnHBCD

