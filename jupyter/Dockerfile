FROM continuumio/anaconda3:4.1.1

MAINTAINER Sajith Appukuttan <asajith@gmail.com>

ENV LANG=C.UTF-8 LC_ALL=C.UTF-8

RUN /opt/conda/bin/conda install numpy  scipy  seaborn matplotlib  statsmodels  scikit-learn jupyter -y --quiet && \
    mkdir /opt/notebooks



ENTRYPOINT [ "/usr/bin/tini", "--" ]
CMD [ "/bin/bash" ]