# Identifying-Entities-in-Healthcare-Data-NLP-Normal Entity Relationship

## Problem Statement
Let’s consider a hypothetical example of a health tech company called ‘BeHealthy’. Suppose ‘BeHealthy’ aims to connect the medical communities with millions of patients across the country.
<br> 

 

‘BeHealthy’ has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions.

<br> 

So, companies like ‘BeHealthy’ are providing medical services, prescriptions and online consultations and generating huge data day by day.

<br> 

Let’s take a look at the following snippet of medical data that may be generated when a doctor is writing notes to his/her patient or as a review of a therapy that he or she has done.

<br>

“The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy.”

 <br>

As you can see in this text, a person with a non-medical background cannot understand the various medical terms. We have taken a simple sentence from a medical data set to understand the problem and where you can understand the terms ‘cancer’ and ‘chemotherapy’. 

 
<br>
Suppose you have been given such a data set in which a lot of text is written related to the medical domain. As you can see in the dataset, there are a lot of diseases that can be mentioned in the entire dataset and their related treatments are also mentioned implicitly in the text, which you saw in the aforementioned example that the disease mentioned is cancer and its treatment can be identified as chemotherapy using the sentence.

 
<br>
But, note that it is not explicitly mentioned in the dataset about the diseases and their treatment, but somehow, you can build an algorithm to map the diseases and their respective treatment.

 <br>

Suppose you have been asked to determine the disease name and its probable treatment from the dataset and list it out in the form of a table or a dictionary like this.

## Tasks Performed
* [Task 1 Data Pre-Processing](#task-1-data-pre-processing)
* [Task 2 Concept Identification](#task-2-concept-identification)
* [Task 3 Defining Features for Conditional Random Field (CRF) Model](#task-3-defining-features-for-conditional-random-field-model)
* [Task 4 Getting the features and the labels of sentences](#task-4-getting-the-features-and-the-labels-of-sentences)
* [Task 5 Defining input and target variables](#task-5-defining-input-and-target-variables)
* [Task 6 Building the CRF Model](#task-6-building-the-CRF-model)
* [Task 7 Evaluation](#task-7-evaluation)
* [Task 8 Identifying Diseases and Treatments using Custom NER](#task-8-identifying-diseases-and-treatments-using-custom-NER)

## Conclusion
In this project I was able to create a custom CRF model sucessfully which was able to extract the diseases and correspondings treatments. The model achieved a `Training F1-Score` of `93.12 %` and `Test F1-Score` of `91.89 %`. Ultimately, I was also able to predict the treatment for `Hereditary Retinoblastoma` which is `Radiotherapy`.
