# Use-DSX-and-Scikit-Learn-to-Predict-US-Opioid-Prescribers
A pattern focusing on how to use scikit learn and python (in DSX) to predict opioid prescribers based off of a 2014 kaggle dataset.

## Use Machine Learning to Predict U.S. Opioid Prescribers with DSX and Scikit Learn

## Intro

This pattern dives into a dataset which looks at opioid overdose deaths by state as well as different, unique physicians, their credentials, specialties, whether or not they've prescribed opioids in 2014 as well as the specific prescriptions they've prescribed. Follow along to see how to explore the data in a DSX notebook, visualize a few initial findings using Pixie Dust, and then use scikit learn to use machine learning to train several models and evaluate which have the most accurate predictions of opioid prescriptions. 

## Architecture Image

![alt text](https://github.com/MadisonJMyers/Use-DSX-and-Scikit-Learn-to-Predict-US-Opioid-Prescribers/blob/master/docs/images/architecture.png)

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

See the template or example journeys for how to include a link to your video with a preview. Say the YouTube video is at `https://www.youtube.com/watch?v=Jxi7U7VOMYg`, that means the video ID is `Jxi7U7VOMYg`. To generate a video preview, add the following snippet, replacing `Jxi7U7VOMYg` with the new video ID:  ``[![](http://img.youtube.com/vi/Jxi7U7VOMYg/0.jpg)](https://youtu.be/Jxi7U7VOMYg)``

## Steps

1. Upload the data to DSX as data assetts (this particular kaggle problem has three datasets).
2. Start a notebook and load the data assetts into it as three seperate pandas dataframes.
3. Explore the different datasets using python, pandas and Pixie Dust.
4. Clean the data using python.
5. Run several models to predict opioid prescribers using scikit learn.
6. Evaluate the models.

For the code, see the notebook found under docs/source/notebooks!

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

