

#start with image of python, alpine is a specific version of linux which is good to use with Docker images
FROM python:alpine3.10  

#working directory for this specific application
WORKDIR /app 

#copy the python code
COPY . /app

#manage dependencies in python -- using pip to download the flask framework
RUN pip install -r requirements.txt

#expose port 5000 to the outside world
EXPOSE 5000

#and launch up the launch.py
CMD python ./launch.py

#COPY requirements.txt /app/requirements.txt
#ENTRYPOINT ["python", "./launch.py"]
