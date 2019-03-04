# Predicting user location based on their reviews
## Objective:
Here we are finding two locations of zomato users, one location is predicted from the restaurants location from which they have taken delivery from and another location is from the restaurants location where they have reviewed to find favorite eating locations.

## Prerequisite
To run the codes the following libraries and dataset need to be downloaded.
* The required python libraries are : `pandas` , `numpy` , `sklearn`  and  `folium` .

* The `jupyter notebook ` must also be installed along with python 3 to run the codes.

  all these libraries can be install via  python `pip` installer.

* The two datasets are required for these they are [zomato_user_reviews.csv](https://drive.google.com/open?id=1NmNNyHcZjMeeQoIQRNTM6_ek886rcxg8) and [resturants_location.csv](https://drive.google.com/open?id=1dUM6G-aKTLfUW17OGy2QBxtFpFB5fmQ6)

## Idea:
1. Two lists are made for each user. One containing the list of all the restaurants from which the user has taken the delivery and other list containing the list of the restaurants which the user has reviewed in zomato.
2. Then from the restaurants location files the coordinates are collected and `DBSCAN` is run on the coordinates and centroid are calculated for each cluster as probable location.
3. Finally, the centroids are plot using python `folium` library which generates a web map containing interactive action.

## Execution:
First run the `user_centroid.ipynb` and then the `plot_map.ipynb` to get the web maps containing the probable location of all the users in `maps` folder. (The `maps` empty folder need to be created before running the `plot_map.ipynb` file.)  
  

  

  
