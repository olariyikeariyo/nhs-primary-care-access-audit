# NHS Primary Care Access Audit

## Overview
An audit of patient access to GP services across England using GP Patient Survey data. The analysis focuses on phone access and appointment satisfaction at Integrated Care Board (ICB) level.

## Problem Statement
Difficulty accessing GP appointments is a major driver of patient dissatisfaction and downstream system pressure. There is significant variation in reported access across ICBs, suggesting uneven operational performance.

## Stakeholders
- NHS England
- Integrated Care System leadership
- GP practice managers
- Primary care commissioners
- Patients and public

## Key Questions
- Which ICBs perform below the national average for phone access?
- How does phone access relate to appointment satisfaction?
- Are there consistent regional patterns of underperformance?

## Data Sources
- **GP Patient Survey – Practice Level Data** (NHS England)  
- **Time period:** Latest published survey year  
- **Coverage and limitations:** Self-reported survey data. One row per GP practice. Does not capture appointment supply or call handling capacity.

## Approach
- Data ingestion and cleaning
- Aggregation from practice to ICB level
- Benchmarking against national averages
- Identification of underperforming ICBs
- Comparative analysis of phone access and appointment satisfaction

## Key Findings
- Multiple ICBs underperform the national average for phone access
- Poor phone access frequently aligns with lower appointment satisfaction
- Performance variation suggests operational drivers rather than patient demographics alone

## Visual Outputs
- ICB benchmark bar charts for phone access  
- Scatter plot of phone access vs appointment satisfaction  
- Summary tables of underperforming ICBs  
(See `/notebooks` and `/outputs`)

## Delivery Considerations
- Survey response bias may affect absolute values
- Results assume comparability across regions
- Digital access channels are not included

## Recommendations
- Prioritise call-handling improvements in lowest-performing ICBs
- Share operational best practice from high-performing regions
- Monitor access metrics alongside satisfaction indicators

## Impact
Improved access to GP services could increase patient satisfaction, reduce repeat contacts, and ease pressure on urgent care services.

## Tools Used
Python pandas numpy matplotlib seaborn VSCode

## How to Run
1. Clone the repository  
2. Install dependencies using `pip install -r requirements.txt`  
3. Place source data in `data/raw`  
4. Run `python run.py`

## Next Steps
- Extend analysis across multiple survey years
- Incorporate appointment volume data
- Include digital access measures
