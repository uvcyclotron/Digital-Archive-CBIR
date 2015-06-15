This code is for extracting 3D color histograms and matching images on the basis of these histograms using a `Chi-squared distance` metric.

- **histogram.py** contains the actual code for generating color histograms of all the images in the database. Python packages for `OpenCV` and `dicttoxml` must be installed to run this code (go through import calls in code for other required packages). You can run this code by typing `python histogram.py -d arg1 -i arg2` where `arg1` is the image database location(should be `../Database/fullsize`) and `arg2` is the XML file where you want to store the 3D histograms(should be `../Database/color.xml`). 

- **search.py** is used for image matching and ranking based on color histogram similarity. It is called inside a python-shell by `Digital_Archive/Client/routes/index.js` where it is essentially being called like `python search.py arg1 arg2 arg3` where `arg1` is the image database location(`../Database`), `arg2` is location of histogram containing XML file(`../Database/color.xml`) and `arg3` is the path to query image. It returns the top 10 image match results. This code can be called independently using the format described.