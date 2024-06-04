## Flight Delay Classification

### Introduction
This is a **group project** for **Course MAT3378 - Big Data Management**.

1. Learning objectives:
  - learn about the dataflow - how data is collected, stored, processed, utilized for analysis, model training and/or other purposes
  - get to know common platforms/technologies/ frameworks for big data related tasks such as Hadoop, Spark, Kafka, etc.
  - hands-on practice for better understanding through bite-size exercises

2. About the project
  - summary: a system to **predict continuously flight delay** at take-off and/or departure
  - topics covered: real-time classification, stream processing, data pipeline, decision tree, gradient boost tree
  - tech stack: Kafka, Spark Structured Streaming, PySpark
  - results:
    + simulated **real-world data stream** and data **processing pipeline**
    + built models with **machine learning classfication** algorithms
    + applied trained models for **making** **inference on streaming data**

### Problem
1. Input
The Flight Delays and Cancellation data was collected and published by the U.S. Department of Transportation’s (DOT) Bureau of Transportation Statistics, 2015. The dataset contains **1,048,574 flight records** with **31 features** representing each flight information. Train/test ratio is divided below: 
  - **75%** for building **models**
    + **90%** for **training**
    + **10%** for **testing**
  - **15%** for demonstrating flight delay **classification**

2. Output
Classified label of ***1 as delayed*** and ***0 as on-time***

### Train models: a total of ***4 models***
1. Classifier
  - Decision Tree
  - Gradient Boost Tree

2. Prediction for
  - Arrival Delay
  - Departure Delay

3. How to load
  - model = PipelineModel.load("models/'model_name'")
