# TB NanoString Shiny App

This is a Shiny app I made to explore TB NanoString gene expression data using PCA, UMAP, NMF, and k-means clustering.

## What the App Does

The app lets you:
- Choose between PCA, UMAP, and NMF.
- Change the number of clusters from 2 to 9.
- See a plot where the clusters have different colors and TB and LTBI samples have different shapes.
- See the cluster centers marked on the plot.
- Look at a table comparing the clusters with TB status.
- See the Adjusted Rand Index (ARI) to check how well the clusters match the actual TB status.

## How to Run the App

1. Download `app.R` and `TBnanostring.rds` from this GitHub repository.
2. Put both files in the same folder on your computer.
3. Open RStudio and install these packages if you don't already have them:

   ```r
   install.packages(c("shiny", "uwot", "NMF", "mclust"))
   ```

4. Open `app.R` in RStudio.
5. Make sure your working directory is the folder where you saved the files. You can check it by typing `getwd()` in the Console.
6. Click **Run App** in RStudio.

## How to Use the App

Once the app opens, you can choose PCA, UMAP, or NMF from the dropdown menu. You can also change the number of clusters to see how the results change.

The plot will show the clusters and TB status, and the table and ARI value will update based on what you select.

The app uses the `TBnanostring.rds` dataset included in this repository.
