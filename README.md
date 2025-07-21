# Structural brain deviations in spinal cord snjury and neuropathic pain

This repository contains code and data analyses for the Master's thesis: **"Normative modeling reveals brain structure abnormalities in spinal cord injury and neuropathic pain"**

**Author**: Valentina Haas
 
International Collaboration on Repair Discoveries, University of British Columbia, Vancouver, BC, Canada


Department of Health Science and Technology, ETH Zurich, Switzerland

*Note: This is all based on an illustrative sample of data, in order to protect patient confidentiality.

##  Project Overview

Spinal cord injury (SCI) often results in motor, sensory, and autonomic dysfunction and is frequently accompanied by neuropathic pain (NP). Traditional neuroimaging studies of SCI are limited by small, unmatched control groups. This project leverages normative modeling to detect individual-level structural brain deviations in SCI, using the [Braincharts framework](https://github.com/predictive-clinical-neuroscience/braincharts/tree/master) trained on over 58,000 healthy controls. 

### Key Goals

- **Quantify cortical thickness and subcortical volume deviations** in SCI participants
- **Explore differences** between SCI participants with (SCI-NP) and without neuropathic pain (SCI-nNP)
- **Correlate structural deviations** with pain intensity and extent

## Methodology

### Normative Modeling Approach
- Utilizes the Braincharts framework with >58,000 healthy control participants
- Individual-level deviation detection from normative brain structure
- Focus on cortical thickness and subcortical volume measurements


### Analysis Pipeline
1. **Data Preprocessing**: Structural MRI data preparation
2. **Normative Model Application**: Extraction of new adjusted SCI values + normative values for analysis (Apply_normative_model_.ipynb)
3. **Calulation of deviations from normative model**: Deviation calculation (new adjusted values - normative values) 
4. **SCI Comparison to normative model**: SCI deviations from the normative model
5. **Group Comparisons**: SCI-NP vs SCI-nNP analysis
6. **Correlation Analysis**: Structural deviations vs clinical pain measures 


## Repository Structure
1. **Apply_normative_model_SCI.ipynb**: Demonstrates how to use Braincharts normative models to estimate individual brain structure deviations in new data, including model adaptation for new sites and extraction of adjusted values + normative values from each feature.
    - Adaption_file_Controls.csv: This is an **illustrative example** file containing structural MRI data (FreeSurfer Outputs) from healthy control participants, including demographic information (e.g., age, sex, site) and detailed cortical thickness and subcortical volume measurements. It is intended to illustrate how to adapt the Braincharts normative model to the specific characteristics of a new dataset or imaging site.
    - Braincharts_SCI_Template.csv: This is an **illustrative example** file providing structural MRI data (FreeSurfer Outputs) for spinal cord injury (SCI) participants. It includes the same types of measurements as the controls file, allowing for demonstration of how to calculate individual deviations from the normative model and perform group analyses. 
    - normative_values_males.xslx: This is the **extracted** file with all the normative values for each age category and centile per feature for the males.
    - normative_values_females.xslx: This is the **extracted** file with all the normative values for each age category and centile per feature for the females. 
      
2. **Final_Brain_Analysis_Braincharts.ipynb**: Performs SCI participant comparisons to the normative model, followed by group comparisons (SCI-NP vs. normative model, SCI-nNP vs. normative model, SCI-NP vs. SCI-nNP), and correlation of brain structure deviations with pain measures.

   Files needed: 
    - Normative_values_males.xslx
    - Normative_values_females.xslx
    - Example_Adjusted_Values_Info.xslx: This includes both the values that have been calculated in step 1 and additional clinical information
