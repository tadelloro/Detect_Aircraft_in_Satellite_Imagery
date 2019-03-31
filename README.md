## Detect Aircraft in Satellite Imagery

#### Problem
The purpose of this project is to detect the location of planes in satellite images collected over airports and other spaces. The automation of satellite image analysis may provide unique insights into various markets such as agriculture, defense, intelligence, energy, and/or finance. The current project is structured as a binary classification problem aimed at labeling each satellite image as containing a plane or not containing a plane. Five Machine Learning algorithms (i.e., Logistic Regression, K-Nearest Neighbors, Random Forest, AdaBoost, and Gradient Boosting), and two Convolutional Neural Networks are optimized, trained, and tested to detect planes in a dataset of 32,000 satellite image chips collected over California.

#### Jupyter Notebooks
* Stage 1 includes data import, exploratory data analysis, and bootstrap hypothesis testing.
* Stage 2 includes model optimization, testing, and comparative results.

#### Report and Presentation
* Final Report includes an abstract, introduction, description of exploratory analysis, learning methods, and results.
* Final Presentation includes a slide deck of key points and take-aways from the study.

#### Datasets
The PlanesNet data are included in the Kaggle dataset “Planes in Satellite Imagery”, provided by Planet Labs Inc. The data are 20x20 images, each with three bands, in a JSON formatted file containing data, labels, scene id's, and location metadata. A total of 32,000 images are provided, the total JSON file size is 191 Mb. Satellite imagery used to build PlanesNet is made available through Planet Labs' Open California dataset, which is openly licensed.

The Kaggle dataset can be found here:
* https://www.kaggle.com/rhammell/planesnet#planesnet.json


| JSON formatted text file | Description                                                                                                                   |
|--------------------------|-------------------------------------------------------------------------------------------------------------------------------|
| data                     | Pixel value data for each 20x20 RGB image is stored as a list of 1200 integers. The first 400 for red, then green, then blue. |
| label                    | Valued 1 or 0, representing the "plane" class and "not-plane" class, respectively.                                            |
| scene id                 | The unique identifier of the PlanetScope visual scene the image chip was extracted from.                                      |
| longitude & latitude     | The longitude and latitude coordinates of the image center point, with values separated by a single underscore.               |

#### Motivating Questions
Can satellite imagery be used to effectively identify aircraft on the ground? How well (in terms of precision and recall) can a deep learning model be tuned to identify planes?

#### Business Case and Clients/Stakeholders
Satellite imagery provides unique insights into various markets, including agriculture, defense and intelligence, energy, and finance. 

#### Deliverables	
* Report and/or article
* Code
* Slide deck

