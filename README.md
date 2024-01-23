HOUSE PRICE ESTIMATION AND CLUSTERING CHALLENEGE

**#House Price Estimation using K-Nearest Neighbors (KNN)**

**Instructions to run the code**

test.csv and train.csv are the raw datasets given.

sample_submission.csv contains the SalePrice of the test data which was already given.

After running KNN(K Nearest Neighbours) a new file SalePrice_Output.xlsx is created which contains the predicted SalePrice.

Clustering is performed on the training data which creates a csv file named cluster.csv. The last column of this csv file has cluster numbers against each row.

To implement  Gradio,a separate Gradio.ipynb file is created.

reduced_train_data.csv and reduced_test_data.csv contain the training and testing data filtered to the 5 most important attributes.

**Loading the data :**
Assign the csv files of training and test data to variables hence creating dataframes.

**Data Preprocessing :**

Attributes where null values exceed the non-null values are dropped.

Replace the null values with mode or mean of the attribute while dealing with object and float data types respectively.

The heatmap of the data shows the attributes which have less effect on the SalePrice.

Combine the test and train data.
One-hot encode the attributes which have object data-type so that they can go into KNN algorithm.
Split the test and train data.

**#KNN Algorithm**

Implement and train a KNN regression model using the training set. Experiment with different values of k and choose the one that provides the best performance (e.g., using cross-validation). Model Evaluation:

Evaluate the model's performance on the testing set using metrics like Root Mean Squared Error (RMSE).

**#Clustering**

Feature Selection:
Choose the features that are most relevant to the clustering objective. Exclude irrelevant or redundant features that might introduce noise.

Use K-Means alogrithm and plot the elbow curve to find the number of clusters parameter k.

Fit the k means algorithm to the data to form clusters.

Plot a 3D graph where the most dependent variables which determin saleprice are the axis

**Provide recommendations** or actions based on the observed trends. For example, if certain features consistently influence house prices, this information can be valuable for real estate stakeholders. **Limitations and Future Work:**

Discuss any limitations of the analysis. Suggest areas for future exploration or improvement. By combining KNN for regression and k-means clustering, you can gain a comprehensive understanding of house price trends and the factors that contribute to houses being grouped together. This integrated approach helps provide richer insights for decision-making in the real estate domain.

**Implementation of KNN on gradio interface**

Select 5-6 attributes which pose a major role in determining sale price of the house.

Prepare the training and test datasets based on this.

Apply KNN and take input of these attributes using gradio interface.
