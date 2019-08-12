# Singularity Container for Banweiss

[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/3394)

This container contains conda: 4.7.11, python:3.7.3, spyder, and the following libraries:

    fortranformat: 0.2.5
    basemap: 1.2.1
    numpy: 1.17.0
    scipy: 1.3.1
    netcdf4: 1.5.1.2
    wrf-python: 1.3.2
    PyNGL: 1.6.1
    PyNIO: 1.5.5
    matplotlib: 3.1.1
    pandas: 0.25.0

To invoke the python interpreter from command line or a script, run 

    singularity exec <path to this container> python [args]

with the same args you would use if running python independantly.

Likewise, you can access spyder with

    singularity exec <path to this container> spyder [args]
