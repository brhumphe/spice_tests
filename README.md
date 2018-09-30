# README
An assortment of notebooks and tests using the [SpiceyPy](https://github.com/AndrewAnnex/SpiceyPy) library to interface with 
the [NAIF SPICE Toolkit](https://naif.jpl.nasa.gov/naif/toolkit.html).

# Installation
Refer to the [SpiceyPy installation instructions](https://github.com/AndrewAnnex/SpiceyPy/blob/master/docs/installation.rst)
Make sure your Python installation is up to date to avoid SSL errors. **Be sure you are using a 64-bit version of 
python!**

# Downloading Data Sets
Datasets can be obtained from the [PDS NAIF Archives](https://naif.jpl.nasa.gov/naif/data_archived.html). 
Use `wget` to download the files at the archive links, using the instructions [here](https://naif.jpl.nasa.gov/naif/download_tip.html)
**Make sure you use _ftp_, not _http_!** For example, to download the Deep Impact SPICE mission data, run the following within the `data` directory:

    wget -m -nH --cut-dirs=5 -nv ftp://naif.jpl.nasa.gov/pub/naif/pds/data/di-c-spice-6-v1.0/disp_1000/

and for Hayabusa:

    wget -m -nH --cut-dirs=5 -nv ftp://naif.jpl.nasa.gov/pub/naif/pds/data/hay-a-spice-6-v1.0/haysp_1000/
