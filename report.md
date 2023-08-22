# Credit Risk Classification Report

## Overview of the Analysis
The purpose of this analysis is to help the nonprofit foundation Alphabet Soup select applicants for funding that have the best chance for success. Alphabet Soup provided a list of more than 34,000 organizations with the following list of metadata:
   - EIN and NAME—Identification columns
   - APPLICATION_TYPE—Alphabet Soup application type
   - AFFILIATION—Affiliated sector of industry
   - CLASSIFICATION—Government organization classification
   - USE_CASE—Use case for funding
   - ORGANIZATION—Organization type
   - STATUS—Active status
   - INCOME_AMT—Income classification
   - SPECIAL_CONSIDERATIONS—Special considerations for application
   - ASK_AMT—Funding amount requested
   - IS_SUCCESSFUL—Was the money used effectively

## Results
### Data Preprocessing
  - The target for the model was IS_SUCCESSFUL
  - The features used were:
    - APPLICATION_TYPE
    - AFFILIATION
    - CLASSIFICATION
    - USE_CASE
    - ORGANIZATION
    - STATUS
    - INCOME_AMT
    - SPECIAL_CONSIDERATIONS
    - ASK_AMT
  - Fields removed from the model were NAME and EIN  

### Compiling, Training, and Evaluating the Model
  - The first layer consisted and 80 neurons while the second layer consisted of 30 neurons
  - The target accuracy of 75% was not achieved
  - Fields were dropped and neurons were increased to increase accuracy but the changes did not yield 75% accuracy
  
## Summary
In summary, the overall accuracy of the results did not meet the 75% threshold for an acceptable model. There were some outliers as to the size of the loans and a deep dive into removing some of those outliers may make the model perform better. There were also two columns, CLASSIFICATION and USE_CASE that seem to be redundant to each other so removing one of those columns would be another possible experiment to improve the performance.  
