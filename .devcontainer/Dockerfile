FROM python:3-slim
EXPOSE 8000

ENV DIRPATH=/workspaces/web-omr

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
   && apt-get -y install git

RUN pip install flask

RUN pip install tensorflow

RUN apt-get install -y python3-opencv
RUN pip install opencv-python

RUN pip install Pillow

WORKDIR $DIRPATH

RUN apt-get -y install wget && apt-get -y install unzip

RUN wget https://grfia.dlsi.ua.es/primus/models/PrIMuS/Semantic-Model.zip
RUN unzip Semantic-Model.zip -d ${DIRPATH}/Semantic-Model
RUN rm Semantic-Model.zip

RUN wget https://raw.githubusercontent.com/OMR-Research/tf-end-to-end/master/Data/vocabulary_semantic.txt -q -o -

#ADD https://www.fontsquirrel.com/fonts/aaargh /Aaargh.ttf

RUN chmod 512 ${DIRPATH}/vocabulary_semantic.txt

