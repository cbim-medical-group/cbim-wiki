# BioBank:

1. Related resources:

1.1 BioBank AMS: https://bbams.ndph.ox.ac.uk/ams/resApplications

1.2 Biobank root path:
/research/cbim/medical/medical-share/private/cardiac/biobank

1.3 Some commands:
  ./ukbconv ukb46169.enc_ukb bulk -s20209
  ./ukbfetch -bukb46169.bulk -s1 -m1000 -of1

    Return 2541
    Application:	2964, Description of cardiovascular phenotype in the UK Biobank population based on cardiovascular magnetic resonance and carotid ultrasound
    Title:	The impact of cardiovascular risk factors on cardiac structure and function: Insights from the UK Biobank imaging enhancement study
    Author:	Petersen, S.E. et al
    Paper:	PLOS ONE. 2017
    URL:	https://doi.org/10.1371/journal.pone.0185114
    Size:	1.5 GB
    Archived:	26 Oct 2020
    Stability:	Updateable
    Personal:	Contains individual-level data


    Contact for queries: a.lee@qmul.ac.uk or s.e.petersen@qmul.ac.uk

    This returned dataset contains CMR data on the first ~5000 participants who attended the imaging enhancement visit. The analysis was using the long axis and short axis CMR cine images

    Returned data contains:

    1) Image derived phenotypes (IDPs):
      • Left atrial two-chamber volume (max)
      • Left atrial two-chamber volume (min)
      • Left atrial four-chamber volume (max)
      • Left atrial four-chamber volume (min)
      • Left atrial biplanar volume (max)
      • Left atrial biplaner volume (min)
      • Left Ventricular end diastolic volume
      • Left Ventricular ejection fraction
      • Left Ventricular end systolic volume
      • Left Ventricular mass
      • Left Ventricular stroke volume
      • Right atrial four-chamber volume (max)
      • Right atrial four-chamber volume (min)
      • Right Ventricular end diastolic volume
      • Right Ventricular ejection fraction
      • Right Ventricular end systolic volume
      • Right Ventricular stroke volume

    2) Quality control scores related to the left ventricle (LV), right ventricle (RV), left atrium (LA) and right atrium (RA)

    3) Segmentation/contour files that can be used together with the corresponding CMR DICOM images that UK Biobank hold. These are in the CVI42 proprietary format ( cvi42wsx) and converted to json format files.

    4) Output files from each participants analysis of the LV/RV/LA/RA using CVI42. They are scientific reports (txt files) and contain far more information than what is often used in research and clinical practice;
    ![image](https://user-images.githubusercontent.com/19438484/193141253-fe1a937d-3b7b-4daa-83fd-ed410498aaa8.png)

    [This basket contains: 40 tabular, 10 bulk, 0 HES record, 0 genetic SNP and 5 dataset fields.]
    Baseline characteristics
        Field ID
    Field title
        31
    Sex
        34
    Year of birth
        52
    Month of birth
    Death register
        Field ID
    Field title
        40000
    Date of death
    ECG at rest, 12-lead
        Field ID
    Field title
        20205
    ECG datasets (Bulk)
    ECG during exercise
        Field ID
    Field title
        6025
    Fitness test results, including ECG data (Bulk)
    Ethnicity
        Field ID
    Field title
        21000
    Ethnic background
    Heart MRI
        Field ID
    Field title
        12624
    Identifier for blood pressure device
        20207
    Scout images for heart MRI - DICOM (Bulk)
        20208
    Long axis heart images - DICOM (Bulk)
        20209
    Short axis heart images - DICOM (Bulk)
        20210
    Aortic distensibilty images - DICOM (Bulk)
        20211
    Cine tagging images - DICOM (Bulk)
        20212
    Left ventricular outflow tract images - DICOM (Bulk)
        20213
    Blood flow images - DICOM (Bulk)
        20214
    Experimental shMOLLI sequence images - DICOM (Bulk)
    Left ventricular size and function
        Field ID
    Field title
        22420
    LV ejection fraction
        22421
    LV end diastolic volume
        22422
    LV end systolic volume
        22423
    LV stroke volume
        22424
    Cardiac output
        22425
    Cardiac index
        22426
    Average heart rate
        22427
    Body surface area
    Ongoing characteristics
        Field ID
    Field title
        191
    Date lost to follow-up
    Pulse wave analysis
        Field ID
    Field title
        12671
    PWA start time
        12673
    Heart rate during PWA
        12674
    Systolic brachial blood pressure during PWA
        12675
    Diastolic brachial blood pressure during PWA
        12676
    Peripheral pulse pressure during PWA
        12677
    Central systolic blood pressure during PWA
        12678
    Central pulse pressure during PWA
        12679
    Number of beats in waveform average for PWA
        12680
    Central augmentation pressure during PWA
        12681
    Augmentation index for PWA
        12682
    Cardiac output during PWA
        12683
    End systolic pressure during PWA
        12684
    End systolic pressure index during PWA
        12685
    Total peripheral resistance during PWA
        12686
    Stroke volume during PWA
        12687
    Mean arterial pressure during PWA
        12688
    Vicorder trace
        12695
    Blood pressure test start time
        12697
    Systolic brachial blood pressure
        12699
    Number of PWA tests performed
        12700
    Vicorder results plausible
        12702
    Cardiac index during PWA
    Reception
        Field ID
    Field title
        53
    Date of attending assessment centre
        54
    UK Biobank assessment centre
        21003
    Age when attended assessment centre
    Datasets
        Dataset ID
    Title
        1362
    Derived variable from cardiac MRI
        1363
    Reference ranges for cardiac structure and function using cardiovascular magnetic resonance (CMR) in Caucasians from the UK Biobank population cohort
        1864
    Cardiac radiomics data returned by application 2964
        1889
    Fully Automated Myocardial Strain Estimation from Cardiovascular MRI-tagged Images Using a Deep Learning Framework in the UK Biobank
        1922
    Cardiac MRI contour files returned by application 2964


1.4 Separate data links:

  TAGGING IMAGING: /research/cbim/medical/medical-share/private/cardiac/biobank/bulks/CineTaggingImages_20212
  
  Long Axis Image: /research/cbim/medical/medical-share/private/cardiac/biobank/bulks/LongAxisHeartImages_20208
  
  Short Axis Image(DICOM): /research/cbim/medical/medical-share/private/cardiac/biobank/bulks/ShortAxisHeartImages_20209/raw
  
  Short Axis All Datasets(tfrecords for tensorflow): /research/cbim/medical/medical-share/private/cardiac/biobank/bulks/ShortAxisHeartImages_20209/processed
  
        biobank_mri,derivate***(Dyssynchrony data), new_biobank_dys_acdc_mm_all(combined all dataset)
        
  Short Axis Image and Label Dataset: /research/cbim/medical/medical-share/private/cardiac/biobank/bulks/ShortAxisHeartImages_20209/processed/ukbb/ukbb_20211011013929
  
  
  
  
