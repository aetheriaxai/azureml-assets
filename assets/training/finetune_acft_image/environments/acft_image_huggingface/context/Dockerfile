# PTCA image
FROM mcr.microsoft.com/aifx/acpt/vision/stable-ubuntu2004-cu117-py38-torch1131:{{latest-image-tag:biweekly\.\d{6}\.\d+}}

USER root
RUN apt-get -y update

# Install required packages from pypi
COPY requirements.txt .
RUN pip install -r requirements.txt --no-cache-dir
