FROM ubuntu:latest
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
RUN pip install --upgrade pip
COPY ./service /MythicalMysfitsService
WORKDIR /MythicalMysfitsService
RUN pip install -r ./requirements.txt
ENTRYPOINT ["python"]
CMD ["mythicalMysfitsService.py"]
