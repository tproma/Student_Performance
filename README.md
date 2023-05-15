## End to End Machine Leanring project

# Problem statement
This project is about how a student's performance (test scores) is affected by other variables such as Gender, Ethnicity, Parental level of education, Lunch and Test preparation course.

# Data Collection
Dataset Source - https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977
The data consists of 8 column and 1000 rows.

# Tech Stack Used
- Python
- Flask
- Machine learning algorithms
- Docker

# Infrastructure Required.
- AWS EC2
- AWS ECR
- Git Actions

# Dataset information
- gender : sex of students -> (Male/female)
- race/ethnicity : ethnicity of students -> (Group A, B,C, D,E)
- parental level of education : parents' final education ->(bachelor's degree,some college,master's degree,associate's degree,high school)
- lunch : having lunch before test (standard or free/reduced)
- test preparation course : complete or not complete before test
- math score
- reading score
- writing score


### Step 1: Clone the repository

```
git clone https://github.com/tproma/Student_Performance.git
```

### Step 2- Create a conda environment after opening the repository

```
conda create -n venv python=3.8 -y
```

```
conda activate venv
```

### Step 3 - Install the requirements

```
pip install -r requirements.txt
```

# AWS CI/CD project
steps:
1. Docker Build checked
2. Github Workflow
3. IAM User In AWS


## Docker Setup In EC2 commands to be Executed

#optinal
```
sudo apt-get update -y
```
```
sudo apt-get upgrade
```

#required

```
curl -fsSL https://get.docker.com -o get-docker.sh
```
```
sudo sh get-docker.sh
```
```
sudo usermod -aG docker ubuntu
```
```
newgrp docker
```

## Configure EC2 as self-hosted runner:

## Setup github secrets:

AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app