---
layout: archive
title: "Data"
permalink: /data/
author_profile: true
---

{% include base_path %}

## Source Data

WMLAD draws administrative records from seven state agencies:

| State Agency | Record type | Key information | Time period | Number of individuals |
|---|---|---|---|---|
| Employment Security Department | Employment records for Unemployment Insurance-eligible jobs | Earnings, hours worked, job characteristics, Unemployment Insurance receipt | 2000-2017 | 7,699,646 workers |
| Dept. of Social and Health Services; Health Care Authority | Client program participation and benefit receipt records | Program participation, benefits received, race/ethnicity, sex, age, residential address | 2010-2017 | 4,968,258 clients |
| Dept. of Health | Records on parents listed on WA birth certificates | Race/ethnicity, sex, age, education, residential address | 2010-2016 | 896,558 parents |
| Sec. of State | Voter records | Voting history, sex, age, residential address | 2006-2016 | 6,084,439 voters |
| Dept. of Licensing | Drivers license registration records | Age, sex, residential address | 2005-2016 | 8,367,317 licensees |
| WA State Patrol | Arrest records | Arrest information | 2000-2018 | 777,416 people arrested |


While there is substantial overlap between the populations covered by each data source, the component datasets of WMLAD represent distinct populations based on the administrative processes that lead individuals to be represented in each set of records. The table below represents the overlap between key WMLAD populations for the time period 2010-2016. Each column represents a key data source, and each row indicates what share of individuals in that data source are also included in a source designated in the column header.



| |Driver’s license holders | Registered voters | Workers | DSHS clients | Parents |
|---|---|---|---|---|---|
| % holding driver’s license | 100% | 83% | 80% | 66%| 87% |
| % registered to vote | 64% | 100% | 57% | 44% | 58% |
| % voted | 50% | 68% | 44% | 28% | 41% |
| % worked | 60% | 55% | 100% | 50% | 72% |
| % DSHS clients | 43% | 37% | 43% | 100% | 58% |
| % new parents | 10% | 9% | 11% | 11% | 100% |



## Data Construction

The UW team contracted with the Research and Data Analysis (RDA) division of Washington State’s Department of Social and Health Services (DSHS) to perform the matching required to construct WMLAD.  RDA has capacity to perform high level, complex matching due to its two decades of experience in building and maintaining DSHS’s integrated client database (ICDB) which combines records across DSHS administrations with outside records from several other agencies, including UI records from ESD and criminal records from the state highway patrol. The project used the [Link King](http://the-link-king.party/) record linkage program, a public-domain application which runs on SAS. Kevin Campbell, the Link King developer, joined RDA for this project and carried out the matching personally. Link King uses a combination of deterministic and probabilistic matching algorithms. The linking process included data standardization, blocking into similar records, identity matching, and quality review. Quality control measures included careful implementation of linkage software with an established pedigree where decision rules were modified for each linkage task based on manual review of random samples of identity groupings. As confirmation, linkage results were generally consistent with expectations given known overlap in clients from linked data sources.


## Data Resources

From the raw data files, the WMLAD team has created a series of processed datasets suitable for analysis. We designate analytic datasets that may be useful for multiple inquiries as “Data Resources” and post static versions of them along with code and documentation.  Data resources to date include:



