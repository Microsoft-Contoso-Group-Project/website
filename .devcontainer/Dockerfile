FROM mcr.microsoft.com/devcontainers/python:1-3.12-bullseye

# Install pip for Python 3.12
RUN python -m pip install --upgrade pip

# Copy requirements.txt and install the packages
COPY requirements.txt .
RUN pip install -r requirements.txt
