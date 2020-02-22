# UC-and-CD-diseases-Classification
Classification of Ulcerative Colitis and Crohn's Disease with Gene Expression data

The data set was downloaded from SSC 2016 website (Original source: ArrayExpress: E-GEOD-3365). The data set contains 126 observations that belong to three classes; 41 healthy individuals, 59 CD patients, and 26 UC patients. There are 312 total attributes which include 309 gene-expression features, age, gender, and ethnicity. The ethnicity was omitted in the analysis since there was only a few observation in all other ethnic groups except for the main group.

### Data Preprocessing
Gene expression data are heavily skewed on the linear scale. The low-expressed genes have very low-intensity values and high-expressed genes have very high-intensity values. Hence, the gene expression data were log-transformed before model fitting (This is a common practice).

### Model fitting
An SVM model was fitted, and grid search CV was used to tune parameters.
