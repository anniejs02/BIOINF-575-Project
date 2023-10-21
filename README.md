# BIOINF-575-Project
BIOINF 575 Project on lung cancer subtyping. The goal of this project is to build and evaluate a mathematical model that can discriminate between two lung cancer subtypes. 

Project Description: 

To build the model we use an unsupervised k-means clustering algorithm (Euclidean distance) of 58 NSCLC tumors using k=2.

To evaluate the model we compute the model accuracy. Accuracy in this case is the percentage of samples that the model assigns to the wrong subtype outof all the samples it classifies.

The data contains 40 adenocarcinoma (AD) samples and 18 squamous cell carcinoma (SCC) samples.

Tasks to Complete: 
1. Load the Data
   
2. Perform clustering - you can use the sklearn.cluster module for this task.

3. Once clusters have been identified, create a DataFrame that contains the 58 sample labels as one column, the cluster number as another column and the subtype given in the dataset (adenocarcinoma or squamous cell carcinoma) as another column.
The information about the subtype for a sample is available in the sample metadata as characteristic.
https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM258551Links to an external site.
It can be retrieved programmatically from the objects created using GEOparse functions.

4. Compute and display the accuracy of this clustering.  

5. Fit the model on half of the data (balanced: 20 AD and 9 SCC) and assign a label to the clusters (AD or SCC), then use the model to predict the cluster/label for the other half of the data.

6. Compute and display the accuracy of the model for the prediction results (testing data).

7. Plot (bar plot) the 3 accuracy values for the model:

(i) train the model on all the data and compute the accuracy of the model on that data

(ii) train the model on half of the data and compute the accuracy of the model on that data

(iii) compute the model accuracy built at point (ii) on the other half of the data (test data)

 

8. As a team decide on a new feature to implement that can answer a relevant biological question using these data and implement the feature
