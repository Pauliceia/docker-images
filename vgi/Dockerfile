FROM python:3

WORKDIR /usr/src/vgiws

COPY ./api/requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
RUN apt-get update
RUN apt-get install -qqy software-properties-common --no-install-recommends
RUN apt-get update
RUN apt-get install -y python-gdal python3-gdal gdal-bin

COPY ./api .

EXPOSE 8888

CMD [ "python", "main.py" ]