<a data-cy="workflow-status-link" href="/pipelines/github/codewheezy/udacity-cloud-devops-p4/10/workflows/936f1a12-2ee2-4479-ab2d-69a506608401" class="css-l59eie"><div title="Success" type="SUCCESS" class="css-t4mprq"><div color="#FFFFFF" class="css-1yz9tv3"><svg role="img" focusable="false" viewBox="0 0 24 24" aria-label="Status Passed" fill="currentColor" xmlns="http://www.w3.org/2000/svg" class="css-bleycz"><path fill-rule="evenodd" clip-rule="evenodd" d="M12 2C6.48 2 2 6.48 2 12C2 17.52 6.48 22 12 22C17.52 22 22 17.52 22 12C22 6.48 17.52 2 12 2ZM10 14.5858L7.70711 12.2929C7.31658 11.9024 6.68342 11.9024 6.29289 12.2929C5.90237 12.6834 5.90237 13.3166 6.29289 13.7071L9.29289 16.7071C9.68342 17.0976 10.3166 17.0976 10.7071 16.7071L17.7071 9.70711C18.0976 9.31658 18.0976 8.68342 17.7071 8.29289C17.3166 7.90237 16.6834 7.90237 16.2929 8.29289L10 14.5858Z"></path></svg></div>Success</div></a>

## Project Overview

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. 

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

Your project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

You can find a detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).

**The final implementation of the project will showcase your abilities to operationalize production microservices.**

---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host. 
# Check the Python path using `which python3`
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
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
