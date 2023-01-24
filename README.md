# ELBARA_L_band_Radiometry_onTP_plot.ipynb
This notebook shows how to access the publised datast of the multiyear L-band microwave radiometry at the Maqu site on the eastern Tibetan Plateau in China, download the data into a folder, read data and process them and plot a figure displaying the seasonal variations of ELBARA-III TB data together with environmental variable (i.e., albedo, air temperature, soil moisture and temperature and ground temperature) data. The produced figure is similar to that in the paper "Multiyear in-situ L-band microwave radiometry of land surface processes on the Tibetan Plateau" published in a Nature Scientific Data Descriptor https://www.nature.com/articles/s41597-020-00657-1. 

The dataset is available at the figshare repository https://doi.org/10.6084/m9.figshare.12058038.v1.
The dataset is fully described in a Nature Scientific Data Descriptor https://www.nature.com/articles/s41597-020-00657-1.



***Script description***

- The Markdown type cell describes the purpose of this Jupyter notebook, 
  the methodology of ELBARA-III radiometry measurement and environmental variable measurements,
  the useful information read from the plotted figure generated by the Jupyter notebook,
  as well as the three directions of dataset applications, supported by already conducted and ongoing researches. 


- The code type cell shows the scripts for computation and plotting. 

  -Package install: install all the required Python packages for computation and plotting. 
  
  -Download dataset from published repository: 1) Type dataset id and base URL; 2) Download data into your folder.
  
  -Fill-in time period for plotting.
  
  -Data processing
  
	-Read ELBARA TB file. In the example,the file 'ELBARA-III dataset-2016-2017ELBARA-III TB.csv' contains two times of header information, 
	 so the script first splits this .csv file into two files for following read for the above filled-in period. 
	 
	-Read in situ automtic weather station measurements, involving air temperature (Tair), precipitation amount, etc,.
	
	   - Process radiation data to get surface albedo data, which is used to reflect the probability of snow events.
	  
	   - Process longwave raidation data to get ground temperature (TG) data.
	  
	-Read in situ soil moisture and soil temperature (SMST) data.
	
	-Plot ELBARA TB data together with environmental variable (i.e., Albedo, SMST, TG, Tair) data. 
	
	  The interpretation of information from the plotted figure can be found at the beginning of this notebook.  
