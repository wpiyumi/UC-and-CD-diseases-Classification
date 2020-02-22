# UC-and-CD-diseases-Classification
Classification of Ulcerative Colitis and Crohn's Disease with Gene Expression data

The data set was downloaded from SSC 2016 website (Original data source: ArrayExpress: E-GEOD-3365). 
The data set contains 126 observations and, they belong to three classes; 41 healthy individuals, 59 CD patients and 26 UC patients. There are 312 attributes; 309 gene-expression data, age, gender and ethnicity. 
Here, ethnisity was not included for the model fitting since there is no enough data to represent all the categories of the ethnicity group.

### Data Preprocessing
Gene expression data are heavily skewed in linear scale. The low-expressed genes have very low intensity values and high-expressed
genes have very high intensity values. Hence, the gene expression data was log transformed before model fitting.

### Model fitting
An SVM model was fitted with 10-fold cross validation. Grid search CV was used to tune parameters.
