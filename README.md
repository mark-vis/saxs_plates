How to use the Jupyter notebook:
* Install Python and Jupyter notebooks. We recommend to install it via the Anaconda environment. See: https://www.anaconda.com/download/ and https://www.askpython.com/python/examples/install-python-with-conda. 
* To run the Jupyter notebook (e.g. the file datasetE72.ipynb), do the following:
	* Open an Anaconda prompt
	* Change locations to the folder where you saved the Jupyter notebook via the following command: cd <folder path>
	* Run Jupyter notebook by typing: jupyter notebook
	* A file overview should open in your browser. Double click the notebook you want to run.
* To run the notebook, you need the following:
	* *.csv file with your averaged and merged SAXS data of the q-range of interest
	* (optional) Pre-calculated form factor table ("P11_table.csv"). Alternatively, you may calculate your own table spanning a range of thicknesses and radii of your own interest. Be aware that the calculation of this form factor table takes rather long depending on the number of data points in there. 


Some tips for a better fit result:
* When your fitting is slow or gives poor results, it might be worthwhile to change the bin size or to eliminate any noisy data ranges in the low- or high-q regions.
* Increasing the resolution of the form factor table, i.e. decreasing the step size, generally improves the fit result. 

Fitting time:
The fitting with a pre-generated form factor table should not take long (ca 7 s for the example data file E72 from the manuscript (gibbsite) run on a 4-year old HP EliteBook 830 G6 with an Intel(R) Core(TM) i7-8665U CPU @ 1.90GHz processor, 32 GB RAM and a 64-bit Windows 11 operating system with an Anaconda Python distribution with Jupyter Notebook version 6.5.2). Be aware that the calculation of a new form factor table takes a number of hours depending on the number of data points in your table.

About:
With this notebook, you may fit scattering data of polydisperse platelets spanning a range of thicknesses L and radii R as is proposed in the manuscript "Morphological analysis of polydisperse nanoplatelets using SAXS" (2024) by L.S. van Hazendonk, R. Tuinier, E. Foschino, L. Matthews, H. Friedrich and M. Vis. Please cite the manuscript when using this script.