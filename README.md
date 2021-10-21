# Clustering-on-a-data-set
Function which performs data clustering and returns a dictionary containing information about the clustered data.
The files contains ;
- id 
- vectors- documents vectors with size 100 from the doc2vec algorithm
- group- document groups(integers from 0 to 9)
I created a cluster_articles function with argument:
- data - a dictionary containing the sae keys as the example dictionary above.
In the cluster_articles functon, i performed a data clustering by running the Kmeans algorithm from the sklearn package on the document vectors with the following arguments: n_clusters = 10, tol=0.05, max_iter= 50,max_iter=50, leaving the rest of the next arguments unchanged
Next, i reduced the dimensionality of the vectors using PCA algorithm with the following arguments:n_components = 10, random_state=2 and then run kmeans on reduced data with the same arguments as above.
The cluster_articles returns a dict with keys
