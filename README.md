[![CircleCI](https://circleci.com/gh/keitamouss/project-ml-microservice-kubernetes.svg?style=svg)](https://circleci.com/gh/keitamouss/project-ml-microservice-kubernetes)

## Project Overview

Operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. 
Main aim of the project is to containerize the python flask-app and deploy the container in Kubernetes cluster. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

* Test project code using linting
* Complete a Dockerfile to containerize this application
* Deploy containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction

---

## Setup the Environment

* Create a virtualenv and activate it

```
python3 -m venv <your_venv>
source <your_venv>/bin/activate
```

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

### Files

* `output_txt_files/docker_out.txt` contains logs returned after running the app with Docker
* `output_txt_files/kubernetes.out.txt` containes logs and the prediction returned after running the app with Kubernetes(`run_kubernetes.sh`)
* `run_docker.sh` contains the steps to get Docker running the app locally
* `run_kubernetes.sh` contains the steps to get Kubernetes running the app locally
* `upload_docker.sh` contains the steps to upload the image to the Docker repository
* `screenshots/activated_virtual_env.png` contains evidence after finish Create and Activate an Environment
* `screenshots/all_tools_version.png` contains all tools (hadolint,docker,kubectl,minikube) version 
* `screenshots/linting_locally.png ` contains evidence status linting locally
* `screenshots/run_docker_log_1.png-run_docker_log_5.png ` contains evidence after run docker script
* `screenshots/make_prediction_docker.png` contains evidence after run docker prediction
* `screenshots/upload_docker_image.png ` contains evidence to built docker image is uploaded in my own personal Docker ID
* `screenshots/minikube_status.png ` contains evidence minikube status
* `screenshots/Cluster_config_view.png ` contains evidence cluster config
* `screenshots/run_kubernetes_script_first_time.png ` contains evidence first time after run kubernetes script
* `screenshots/run_kubernetes_script_second_time.png ` contains evidence second time after run kubernetes script
* `screenshots/make_prediction_kubernetes.png ` contains evidence after run kubernetes prediction
