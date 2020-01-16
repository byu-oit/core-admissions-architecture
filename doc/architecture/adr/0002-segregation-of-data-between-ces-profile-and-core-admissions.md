# 2. Segregation of data between CES Profile and Core Admissions

Date: 2020-01-15

## Status

Proposed

## Context

There are three different types of data associates with the Admissions process. 
- Applicant owned data - Data that is owned by the applicant and should be under their control - Transcripts, test scores, etc
- Common admissions data - Data the applicant has entered into the Core Admissions system - Question answers, etc
- Institutional private data - Data that has been processed or derived in order to make an admissions decision. Endorsement decision, etc. This data may different for each institution. 

## Decision

Applicant owned data resides in the CES Profile (MyInfo) system and the student must grant consent for the data to be shared with the admissions system and admitting
institutions. 
Common admissions data resides within the CES Core Admissions system and is used by each institution's decision processing system. 
Institutional private data resides within each institution's decision processing system. 

## Consequences

- Student owned data is shared only with the student's consent
- Each institution's decision processing system will keep some data that is used by all institutions, hence duplicating the data. 
- Admission decisions will be pushed from each institution's decision processing system back to the Core Admissions system. 
- Each institution, during the onboarding process, will need to access the Core Admissions and CES Profile systems to get a complete picture of the new student. 
- Each institution's decision processing system will call the Core Admissions and CES Profile systems to get the individual views of an applicant. 
