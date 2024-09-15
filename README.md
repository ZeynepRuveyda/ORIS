# Project Overview

In this repository, **traditional machine learning** and **computer vision** models were used to meet the technical test requirements. **Two different solutions** were achieved through these approaches, and the **computer vision model provided a better result**.

## Machine Learning Approach
During the analysis and the **Exploratory Data Analysis (EDA)** phase, I verified the images using **Google Maps links**. However, I found that **Google had incorrectly labeled some of these sites**, indicating that classification using these links was not feasible. Additionally, using the website information was also impractical. Although some names included the word **'carrière'**, not all of them referred to a quarry in the context required. For example, `'carrière-palet.com'` contains the word **'carrière'**, but it is not a quarry.
I tried to use Machine Learning basic methods to see we can achive good results with just one feature even though we can clearly see in the  begining. So that results were really bad. So I did not continue too much machine learning modeling parts to not lose my time.  Based on the results obtained the document **`y_test_ML.csv`** was generated.

On the other hand, an **NLP method** can be applied to the homepage information. By analyzing the word **'carrière'** and related terms or phrases, it might be possible to identify if a site is a quarry. This approach can be further explored in future project iterations. Additionally, this method can be extended to **address information** to identify the official status of the companies, aiding in the prediction of **'Quarry'** or **'Not Quarry'**.

As a result, in the **machine learning model**, the **longitude and latitude columns** were primarily used to draw conclusions.

## Computer Vision Approach
Using the **computer vision model**, an analysis of the images was conducted. **Pytorch** was utilized, and after adjusting specific hyperparameters, an **F1 score of 80%** was achieved. The file **`y_test_CV.csv`** related to this computer vision model can be found in the data folder. The computer vision algorithm can be further improved. By enriching the training data using **Active Learning Methods**, better results can be achieved.
