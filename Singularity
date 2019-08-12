Bootstrap: docker
From: centos:7

%post
    yum groupinstall -y "Development tools"
    yum install -y wget
    yum install -y libcurl-devel zlib-devel
    
    #Spyder x11 requirements
    yum groupinstall -y x11
    yum install -y libXScrnSaver-1.2.2-6.1.el7
    

    wget https://repo.anaconda.com/archive/Anaconda3-2019.07-Linux-x86_64.sh
    bash Anaconda3-2019.07-Linux-x86_64.sh -b -p /opt/anaconda
    export PATH="/opt/anaconda/bin:$PATH"
    source /opt/anaconda/bin/activate

    conda install -c conda-forge fortranformat basemap numpy scipy netcdf4 wrf-python pyngl pynio matplotlib pandas

%environment
    export PATH="/opt/anaconda/bin:$PATH"
    source /opt/anaconda/bin/activate

%help
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


