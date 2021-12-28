# Create image based on Python 3.6

FROM python:3.6


# Tell Python to not generate .pyc

ENV PYTHONDONTWRITEBYTECODE 1


# Turns off buffering for easier container logging

ENV PYTHONUNBUFFERED 1


# Set working directory

WORKDIR /backend


# Copy requirements file

COPY requirements.txt ./


# Install requirements using pip

RUN pip install -r requirements.txt


# Copy flask app to working directory

COPY app.py ./


# set flask environment as developemnt 

ENV FLASK_ENV=development


# Expose ports

EXPOSE 5000


# Start the flask app

CMD python app.py