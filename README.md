# DominantColors

## Synopsis
This is a small project which makes use of Clustering Algorithm, K-Means to create color clusters in input image. The color clusters are visualized using scatter plot and pie-chart. Both input image and number of clusters can be passed in as cmd argument. By default, for input image, it looks into "images" folder which has some sample images while the number of clusters is 5.

## Installation
1. [Pillow](https://pypi.org/project/Pillow/ "Pillow")
2. [Matplotlib](https://matplotlib.org/ "Matplotlib")
3. [Numpy](https://numpy.org/ "Numpy")
4. [collections](https://docs.python.org/3/library/collections.html "collections")
6. [scikit-learn](https://scikit-learn.org/stable/ "Scikit-learn")
7. [Pandas](https://pandas.pydata.org/ "Pandas")
8. [webcolors](https://pypi.org/project/webcolors/ "webcolors")
9. [math](https://docs.python.org/2/library/math.html "Math")
10. [json](https://docs.python.org/3/library/json.html "Json")
11. [argparse](https://docs.python.org/2/library/argparse.html#module-argparse "Argparse")

## Use Case
Android Developers, Web Developers or anyone looking to replicate a template face the problem of identifying the hex codes for colors used in the templates. This program will make their lives easier. They can load the template image in the program, set the number of clusters (No. of colors to be identified) and the program will return the hexcodes and name (actual/nearest) of the colors used in the image.

## Output

### 3D Scatter Plot (different color clusters)
![picture alt](https://i.imgur.com/6U9dP9r.jpg)

### PieChart distribution
![picture_alt](https://i.imgur.com/iUGSCDH.jpg)

## Shortcomings
The name of colors may change with increasing/decreasing number of clusters. This is because the program uses the center of clusters to calculate the hex codes. For color names, it looks up in a JSON containing hexcodes and respective color names. If it is not able to find hex code in the JSON, it finds the nearest hex code (using Euclidean distance) and returns the name of that hex code. When we increase/decrease the number of clusters, the center of cluster changes. Because of that, hex code changes and eventually, the nearest hex code/color name.

Please find the Android App deployment of the program : https://play.google.com/store/apps/details?id=com.proxima.colorpixor

## Contribution
Feel free to fork and submit bug fixes or new features. You can file bugs, suggestions, and feature requests through issues page.
