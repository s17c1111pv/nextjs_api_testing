# backend/blog_prj/Dockerfile
# set base image
FROM python:3.8.7

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# set work directory
WORKDIR /code

# install dependencies
COPY ./blog_prj/requirements.txt ./
RUN python3 -m pip install --upgrade pip setuptools
RUN pip install -r requirements.txt

# Copy project
COPY ./blog_prj/ ./

# Expose application port
EXPOSE 8000