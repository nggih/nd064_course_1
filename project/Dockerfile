FROM python:2.7

LABEL maintainer="Linggih Saputro"

# copy files in the current directory to /app directory in the container
COPY /techtrends /app

# defines the working directory within the container
WORKDIR /app

RUN pip install -r requirements.txt

CMD ["python", "init_db.py", "&&", "python", "app.py"]

# to build use using the Dockerfile from the current directory
# docker build -t python-helloWorld .

# build an image using the Dockerfile from the lesson1/python-app directory
# docker build -t python-helloWorld lesson1/python-app

# run the python-helloWorld image, in detached mode and expose it on port 5111
# docker run -d -p 5111:5000 python-helloworld

# run docker ps to get the container ID
# docker logs {{ CONTAINER_ID }}

# to push to the dockerHub
# docker tag python-helloworld nggih/python-helloworld:v1.0.0
# docker push nggih/python-helloworld:v1.0.0
