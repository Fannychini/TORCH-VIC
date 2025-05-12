# TORCH-VIC: Transforming Outcomes through Research in Cancer Healthcare in Victoria

This repository presents the TORCH-VIC data resource and provides all scripts used to clean, wrangle, and consolidate the linked data collections into a comprehensive data asset for real-world cancer research studies.

## Overview

The Transforming Outcomes through Research in Cancer Healthcare in Victoria (TORCH-VIC) cohort was established in 2022 in response to a pressing need for comprehensive real-world evidence on the cancer care continuum in Australia. 

With the introduction of novel therapies and increasing treatment complexity, there are significant gaps in understanding the real-world cancer care continuum in Australia.

## Primary Aims

To address these gaps, the TORCH-VIC cohort was established with four key objectives:
1. Determine the type and frequency of diagnostic tests and treatments used in contemporary Victorian clinical practice
2. Estimate the costs of cancer care for patients and payers
3. Identify disparities in access and provision of care across different population groups
4. Study adverse events and comorbidity in the cancer setting

## Cohort Design and Population

TORCH-VIC employs a retrospective, population-based design with person-level administrative and registry data for all adults (18+ years) diagnosed with:

- Colorectal cancer
- Lung cancer
- Melanoma
- Prostate cancer
- Breast cancer
- Lymphoid leukemia

The cohort covers all diagnoses in Victoria, Australia, from 2010 to 2021, comprising **222,332 individuals** with **237,089 cancer registrations**.

## Data Linkage Framework

TORCH-VIC leverages a robust cross-jurisdictional linkage capability across Victorian (Centre for Victorian Data Linkage - CVDL) and Commonwealth (Australian Institute of Health and Welfare - AIHW) data collections.

The Victorian Cancer Registry (VCR) serves as the spine of linkage, with people retrospectively identified and linked across the following collections:

### Victorian Data Sources (via CVDL)
| Data Source | Acronym | Period | Description |
|-------------|---------|--------|-------------|
| Victorian Cancer Registry | VCR | Jan 2010 - Dec 2021 | Population-based cancer registry with comprehensive diagnostic information |
| Victorian Admitted Episodes Dataset | VAED | Jan 2010 - May 2023 | Hospital admissions in public and private settings |
| Victorian Emergency Minimum Dataset | VEMD | Jan 2010 - May 2023 | Emergency department presentations |
| Victorian Integrated Non-Admitted Health | VINAH | Jan 2010 - May 2023 | Non-admitted services including outpatient care |
| Victorian Radiotherapy Minimum Data Set | VRMDS | Jan 2010 - May 2023 | Radiotherapy treatments in public and private settings |
| Victorian Death Index | VDI | Jan 2010 - May 2023 | State-level mortality data |
| Elective Surgery Information System | ESIS | Jan 2010 - May 2023 | Elective surgery waiting list data |
| Victorian Cost Data Collection | VCDC | Jan 2010 - Dec 2022 | Patient-level cost data for hospital services |

### Commonwealth Data Sources (via AIHW)
| Data Source | Acronym | Period | Description |
|-------------|---------|--------|-------------|
| Pharmaceutical Benefits Scheme | PBS | Jan 2008 - June 2023 | National prescription medicine dispensing data |
| Medicare Benefits Schedule | MBS | Jan 2008 - June 2023 | National medical service claims data |
| National Death Index | NDI | Jan 2008 - Dec 2022 | National mortality data with cause of death |

## Repository Structure

```
TORCH-VIC/
├── scripts/
│   ├── preprocessing/         # Data cleaning and wrangling scripts
│   ├── merge/                 # Data linkage validation scripts
│   ├── analysis/              # Analysis templates for common use cases
│   └── visualisation/         # Visualisation tools
├── documentation/             # Data elements and proxy definitions
├── examples/                  # Example analyses and use cases
└── README.md                  # This file
```
