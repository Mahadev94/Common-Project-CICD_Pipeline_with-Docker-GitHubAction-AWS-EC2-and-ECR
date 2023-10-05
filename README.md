# This is the END TO END ML PROJECT Pipeline-->By Mahadev94
# Diamond-Price Prediction-gemstone dataset:
## Problem Statement
 You are provided with the dataset containing the prices and other attributes of almost 27,000 cubic zirconia (which is an inexpensive diamond alternative with many of the same qualities as a diamond). The company is earning different profits on different prize slots. You have to help the company in predicting the price for the stone on the basis of the details given in the dataset so it can distinguish between higher profitable stones and lower profitable stones so as to have a better profit share. Also, provide them with the best 5 attributes that are most important.

## Task you can perform 📝
📌 Clean and preprocess the data
📌 Do Exploratory Data Analysis (EDA) to get some insight into data
📌 Do Feature Engineering
📌 Build a model i.e Regression Analysis
📌 Evaluate the model
📌 Go back to any of the previous steps unless the result is sufficient.

## 1. first we have create conda environment in local sys:
conda create -p venv python=3.8
conda activate venv/

## 2. create .gitignore file-->add venv 
 which ever files/folders we dont want to update with github

## install required libraries:

-->requiremts.txt file created to add requireed lib:
pip install -r requirements.txt

-e . -> to trigger setup.py file to add packages in env.


## 3. git hub commands:
 git init
 git add .
 git commit -m "comment which erver you have added"
 git branch -M main
 git remote add origin HTTP....
 git push -u origin main

 ## 4. Project structure:-->
    1. create setup file->
    add function to retrive automatic all requirements from requirements.txt file.
    
    2. notebook -->ipynb file
    3. House-Price--> folder has:
    components:
    exception:
    logging:
    config:
    pipeline:
    utils:
     
## 4. run setup file to install all created packages:
    python setup.py install

    -e . used in requirements.txt file file to install all pachaked in env.
    with pip list we can see it

    5. constant:
    Dockerfile:
    .dockerignore:

## Detailed steps for deployment:
1. Docker Build checked:created docker file and build docker image
2. Github Workflow:crate from Actions->workflow->confugure and commit ot on github.
3. Iam User In AWS:create user and dounload credential csv file.
4. 
## Docker Setup In EC2 commands to be Executed
#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

## Configure EC2 as self-hosted runner:
### Setup github secrets:
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>> 566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app


