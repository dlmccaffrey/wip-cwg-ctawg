# docker build --rm --tag wip-cwg-ctawg .

# start with datascience notebook
FROM jupyter/datascience-notebook

# add nltk and html2text
#python 3
RUN conda install -y nltk
RUN pip install html2text
RUN python -m nltk.downloader all

#python 2
RUN conda install --name python2 -y nltk
RUN pip2 install html2text
RUN /opt/conda/envs/python2/bin/python -m nltk.downloader all