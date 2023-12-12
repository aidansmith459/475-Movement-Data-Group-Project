# 475 Movement Data Group Project
 This project is performing clustering on a set of movement data to determine where the "staying points" are and how long the person stays at those points.


Directiories:

"./" - The main directory contains the notebooks and R files used for our data cleaning, filtering, and clustering

"CleanData" - This directory contains the entire movements.csv dataset split by user with the datetime column split into two

"FilteredData" - This directory contains the results for filtering for the movements_0 file (this file contains the data for id=I000)

"ClusterResults" - This directory contains geojson files that have the cluster results from hbdscan

"Visualization" - This directory contains the html files that make use of the Mapbox GL API in order to create an interactive cluster map from the geojson files in the "ClusterResults" directory


NOTE: in order to launch the html files in the "Visualization" directory, make sure to use LiveServer in VSCode in order to get around CORS restrictions for loading local files through Mapbox.


Naming convention for files: <sample>_<filter method>_<data modification>_<id>.ext (i.e. for a file that shows the filter results of a one day sample from user0 using the round method, the file name would be "day_round_filtered_0.csv")

