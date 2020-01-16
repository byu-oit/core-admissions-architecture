# 3. use CashNet for application payment processing

Date: 2020-01-16

## Status

Accepted

## Context

The current admissions system uses BYU's Payment Manager to process payments from applicants. This is possible because the current system requires each applicant to create 
a BYU identity as part of the application process. A requirement for the new system is that applicants do not create BYU identities until as some point they need to do so because they are applying for other BYU services. 

## Decision

BYU's Payment Manager uses CashNet as its credit card processor. For CES purposes we will use BYU's CashNet instance as the credit card processor for the application fees. This removes the requirement for a BYU identity. 

## Consequences

- There are a number of BYU campus entities that use CashNet directly so this is not a new pattern. It does imply that we will have to develop some of the back end processing and interface that Payment Manager would be supplying. 
- This removes the requirement for a BYU identity. 
