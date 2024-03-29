# Where do objects go on the sea floor?
Repo for earth lab capstone project. 
### Questions
Where do objects go on the ocean floor? 
Hazardous objects are unidentified all over the sea floor. What are the spatial patterns that we might see when using machine learning and artificial intelligence to identify such objects? Furthermore, will these objects be buried in sediment or will they move over time? 

### Goal
The goal of this project is to create a heat map of where objects are off the coast of North and South Carolina in the United States and to predict where they may move. 

This notebook will combine data from various different sources to gather information on where sea floor objects are located. Some of these objects may be hazardous and the hope is that this codebase can predict movement patterns and be used to mitigate risk of hazardous chemicals being released. 

The functions and work created here will display data for the region we've discussed. A user could use the functions here to load in data from sources for different regions/locations.

## Requirements

Python(Jupyter notebook) + Conda

## Usage

1. Download Artifical Reef KMZ [here](https://deq.nc.gov/marine-fisheries/coastal-fishing-information/artificial-reefs/reef-kmz-file/open)
2. Change the extention to `.zip`
3. Unzip the file - it will return a `.kml` and a `.xsl`. Rename the KML to `Reef_Material.kml` and move it to `~/earth-analytics/data/earthpy-downloads/`

All images are held in the `img` directory.

### Data
This repository uses these types of input data:
- KML
- TIF

### Runtime instrctions  
First you will want to navigate to the directory where you have cloned the repository from github.  
Then activate the conda environment - `conda activate seafloor-objects` (if the environment doesn't exist yet first run `conda env create -f environment.yml`).  
The environment.yml lists out all of the packages to be installed in the conda environment.  
This can be run by selecting `run all` at the top of the jupyter notebook as long as the conda environment is activated.

### Docker Instructions
First download docker desktop if you do not have this installed on your computer. 
Open a terminal and use the command "docker pull Seafloor-Objects (latest is our default tag).
Next, use the command "docker run Seafloor-Objects." The container is now active. 
To access the notebook, open the container on docker desktop. Press "run" and under optional settings use port 2:8888. This will open up Jupyter notebook and prompt for a token. This token can easily be found within the docker desktop terminal in the https link. Once the token is added the software will be available. 
For more customized commands in docker see their documentation at https://docs.docker.com/engine/reference/commandline/cli/


## License
See [License](https://github.com/rmarowitz/seafloor-objects/blob/main/LICENSE)

## Credit
This software was developed by Robyn Marowitz and Allison Buchanan
[![DOI](https://zenodo.org/badge/627546755.svg)](https://zenodo.org/badge/latestdoi/627546755)

