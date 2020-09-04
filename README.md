[![circleci](https://circleci.com/gh/Codedkate/Devtest.svg?style=svg)](https://circleci.com/gh/Codedkate/Devtest)

## Project Overview

This project operationalizes a Machine Learning Microservice API. 

Given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

The following tasks were performed:
* Test project code using linting
* Complete Dockerfile to containerize the application
* Deploy the containerized application using Docker and make a prediction
* Improve the log statements in the source code
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested


---
### Short description of folders and files in the repo

* model_data : this folder contains the pretrained `sklearn` model and housing csv files
* output_txt_files: contains sample output logs from running `./run_docker.sh` and `./run_kubernetes.sh`
* app.py : contains the flask app
* Dockerfile: contains instructions to containerize the application
* Makefile : contains instructions on environment setup and lint tests
* requirements.txt: lists environment dependencies
* upload_docker.sh: bash script to upload the application to Dockerhub
* run_docker.sh: bash script to run the application in Docker
* run_kubernetes.sh: bash script to run the application in Kubernetes
* make_prediction.sh: bash script to make predictions
* README.md: this READme file

### Instructions
## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
