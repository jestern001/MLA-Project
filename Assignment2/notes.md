## Example 1: PCA then Clustering
    1) Data Prep
        A) Load data into a dataframe
        B) Drop meaningless columns (ex: 'id')
        C) Rename columns
        E) Convert catagorical varibles into dummy varibles
        F) Handle missing data
        G) Split into X and Y
        H) Standardize/normalize X
    2) PCA
        A) I select "Heart_Disease_Stage" as my target feature.
        B) I use PCA to see which features most impact Y (explain X percent of variance)
        C) Save principal components
    3) Clustering (of principal components)
        A) Get optimal K
            a) Pick a number J of K's to check for the best K
            b) Save inertia for each K=J
            c) Plot inertias and look for the elbow (use yellowbricks if elbow isn't obvious)
        B) Run KMeans for best k and save clusters
        C) Add clusters to dataset
    4) Visualize
        A) Plot Principal Component (PC) 1 vs PC 2 with cluster assignment
## Example 2: Clustering then PCA

