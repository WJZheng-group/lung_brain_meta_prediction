## The following scripts describe how the structured EHR data was processed for machine learning model development:
patient2dict --> more_feature_extraction --> pretraining-labeling --> case_control_matching --> convert4training --> dataset_setup

- Step 1: patient2dict
extract useful columns from each file, and convert it into directionary format.
    
- Step 2: more_feature_extraction
extract lab test and clinical events and save it
    
    
- Step 3: pretraining-labeling
Detect the datetime of lung cancer, BM, BM_facts, hospice and expired encounter;
    
- Step 4: case_control_matching
    
- Step 5: convert4training
Extract information to be sent for training, and convert the format;
Add more features, like clinical events and lab test;
    
- Step 6: dataset_setup_retain
Further clean the data, and make input for RETAIN model;
    
    
RETAIN model is forked from [https://github.com/mp2893/retain]
