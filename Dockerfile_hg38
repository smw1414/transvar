FROM python:2.7

LABEL maintainer="Shao-Min Wu" \
      contact="hdf87ery@hotmail.com"
	  
 # Define working directory.
RUN mkdir /data -p

RUN pip install transvar
RUN transvar config --download_anno --refversion hg38
# in case, if you don't have a reference
RUN transvar config --download_ref --refversion hg38
# in case you do have a reference to link

WORKDIR /data