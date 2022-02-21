FROM jupyter/scipy-notebook:python-3.2.0

MAINTAINER Fernando Dorado <fernando.dorado.rueda@idener.es>


# Install from requirements.txt file
COPY requirements.txt /tmp/
RUN pip install --upgrade pip
RUN pip install --requirement /tmp/requirements.txt 
RUN conda install -c conda-forge jupyter_contrib_nbextensions

USER root
RUN chmod -R 777 /usr/local/share/ 

