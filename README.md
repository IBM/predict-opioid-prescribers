# Use-DSX-and-Scikit-Learn-to-Predict-US-Opioid-Prescribers
A pattern focusing on how to use scikit learn and python (in DSX) to predict opioid prescribers based off of a 2014 kaggle dataset.

## Use Machine Learning to Predict U.S. Opioid Prescribers with DSX and Scikit Learn

## Intro
Opioid prescriptions and overdoses are becoming an increasingly overwhelming problem for the United States, even causing an official state of emergency in recent months. Though we, as data scientists, may not be able to single handedly fix this problem, we can dive into the data and figure out what exactly is going on and what may happen in the future given current circumstances.

This pattern aims to do just that: it dives into a kaggle dataset which looks at opioid overdose deaths by state as well as different, unique physicians, their credentials, specialties, whether or not they've prescribed opioids in 2014 as well as the specific prescriptions they've prescribed. Follow along to see how to explore the data in a DSX notebook, visualize a few initial findings geographically and otherwise using Pixie Dust, and then use scikit learn to use machine learning and train several models to figure out which have the most accurate predictions of opioid prescriptions. 

## Architecture Image

![alt text](https://github.com/MadisonJMyers/Use-DSX-and-Scikit-Learn-to-Predict-US-Opioid-Prescribers/blob/master/docs/source/images/architecture.png)

## Flow

1. Log in to or start a DSX account.
2. Upload the data as a data asset into DSX.
3. Start a notebook in DSX.
4. Input the data into your notebook from your data assets.
5. Explore the data with python pandas and Pixie Dust.
6. Train machine learning models with scikit learn.
7. Evaluate their prediction performance.

## Included components

* [IBM Data Science Experience](https://www.ibm.com/bs-en/marketplace/data-science-experience): Analyze data using RStudio, Jupyter, and Python in a configured, collaborative environment that includes IBM value-adds, such as managed Spark.
* [Jupyter Notebook](http://jupyter.org/): An open source web application that allows you to create and share documents that contain live code, equations, visualizations, and explanatory text.
* [PixieDust](https://github.com/ibm-watson-data-lab/pixiedust): Provides a Python helper library for IPython Notebook.

## Featured technologies

* [Data Science](https://medium.com/ibm-data-science-experience/): Systems and scientific methods to analyze structured and unstructured data in order to extract knowledge and insights.
* [Python](https://www.python.org/): Python is a programming language that lets you work more quickly and integrate your systems more effectively.
* [pandas](http://pandas.pydata.org/): A Python library providing high-performance, easy-to-use data structures.

## Watch the Video

TBD

## Steps

    1. Sign up for the Data Science Experience.
    2. Create a notebook and load the data assetts into it as three seperate pandas dataframes.
    3. Upload the data to DSX as data assetts (this particular kaggle problem has three datasets).
    4. Explore the different datasets using python, pandas and Pixie Dust.
    5. Clean the data using python.
    6. Run several models to predict opioid prescribers using scikit learn.
    7. Evaluate the models.

1. Sign up for the Data Science Experience

Sign up for IBM's Data Science Experience. By signing up for the Data Science Experience, two services: DSX-Spark and DSX-ObjectStore will be created in your Bluemix account. If these services do not exist, or if you are already using them for some other application, you will need to create new instances.

To create these services:

    Login to your Bluemix account.
    Create your Spark service by selecting the service type Apache Spark. If not already used, name your service DSX-Spark.
    Create your Object Storage service by selecting the service type Cloud Object Storage. If not already used, name your service DSX-ObjectStorage.

    Note: When creating your Object Storage service, select the Swift storage type in order to avoid having to pay an upgrade fee.

Take note of your service names as you will need to select them in the following steps.

 
2. Create a notebook and load the data assetts into it as three seperate pandas dataframes.

First you must create a new Project:

    From the IBM Data Science Experience page either click the Get Started tab at the top or scroll down to Recently updated projects.
    Click on New project under Recently updated projects.
    Enter a Name and optional Description.
    For Spark Service, select your Apache Spark service name.
    For Storage Type, select the Object Storage (Swift API) option.
    For Target Object Storage Instance, select your Object Storage service name.
    Click Create.

Create the Notebook:

    Click on your project to open up the project details panel.
    Click add notebooks.
    Click the tab for From URL and enter a Name and optional Description.
    For Notebook URL enter: https://github.com/IBM/spark-tpc-ds-performance-test/blob/master/notebooks/run-tpcds-on-spark.ipynb
    For Spark Service, select your Apache Spark service name.
    Click Create Notebook.
3. Upload the data to DSX as data assets (this particular kaggle problem has three datasets).

 To begin, I used the included data as my three data assets. You'll want to upload each as a data asset and once that is    complete, go into your notebook in the edit mode (click on the pencil icon next to your notebook on the dashboard). To load your data in your notebook, you'll click on the "1001" data icon in the top right. The combined_data.csv should show up. Click on it and select "Insert Pandas Data Frame". Once you do that, a whole bunch of code will show up in your first cell. 
 
4. Explore the different datasets using python, pandas and Pixie Dust.
5. Clean the data using python.
6. Run several models to predict opioid prescribers using scikit learn.
7. Evaluate the models.

For the code, see the notebook found under docs/source/notebooks or view the notebook here: https://dataplatform.ibm.com/analytics/notebooks/c32975c1-3994-42cc-8e2d-3f579ceebf63/view?access_token=cdb14a077ed4746b09b1dbaa05aee70133589f001dbb7582ba4e7fcfdd73a905!

## Sample output

After running various classifiers, we find that Random Forest, Gradient Boosting and our Ensemble models had the best performance on predicting opioid prescribers.

## Links

 - DSX:https://datascience.ibm.com/docs/content/analyze-data/creating-notebooks.html.
 - Pandas:http://pandas.pydata.org/
 - Pixie Dust: https://ibm-watson-data-lab.github.io/pixiedust/displayapi.html#introduction
 - Data: https://www.kaggle.com/apryor6/us-opiate-prescriptions/data
 - Scikit Learn: http://scikit-learn.org/stable/

## License

 Copyright 2017 IBM Corp. All Rights Reserved.

  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.

