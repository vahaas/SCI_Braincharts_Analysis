# Structural Brain Deviations in Spinal Cord Injury and Neuropathic Pain

This repository contains code and data analyses for the Master's thesis:

**"Structural brain deviations in spinal cord injury and neuropathic pain"**  
 Valentina Haas – ETH Zurich (2025)

##  Project Overview

Spinal cord injury (SCI) often results in motor, sensory, and autonomic dysfunction and is frequently accompanied by neuropathic pain (NP). Traditional neuroimaging studies of SCI are limited by small, unmatched control groups. This project leverages normative modeling to detect individual-level structural brain deviations in SCI, using the Braincharts framework trained on over 58,000 healthy controls.

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
2. **Normative Model Application**: Deviation calculation using Braincharts
3. **Group Comparisons**: SCI-NP vs SCI-nNP analysis
4. **Correlation Analysis**: Structural deviations vs clinical measures

## Expected Outcomes

- Individual-level brain structural deviation maps for SCI participants
- Comparative analysis between pain and non-pain groups
- Correlation matrices linking structural changes to pain characteristics
- Statistical significance testing for group differences

## Research Significance

This study addresses limitations in current SCI neuroimaging research by:
- Using large-scale normative data for comparison
- Providing individual-level rather than group-level analyses
- Investigating the specific relationship between structural changes and neuropathic pain

## Repository Structure
