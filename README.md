
# **Data Mining Analysis on students performance**


## **Dataset Overview**
The dataset contains information on **student performance in academic subjects** based on various demographic and socio-economic factors. It consists of **1,000 student records** with details on gender, parental education, lunch status, test preparation, and scores in math, reading, and writing.



## **Dataset Source**
The dataset is publicly available and typically sourced from educational research databases. It aims to analyse the impact of various factors on student performance.



## **Variables in the Dataset**
The dataset comprises **8 attributes** with categorical and numerical data:

1. **Gender** _(String)_ – Student's gender (Male/Female).
2. **Race/Ethnicity** _(String)_ – Student’s ethnic background (categorized into groups).
3. **Parental Level of Education** _(String)_ – The highest education level attained by the student's parent(s).
4. **Lunch** _(String)_ – Student’s lunch type (standard or free/reduced).
5. **Test Preparation Course** _(String)_ – Whether the student completed a test preparation course (yes/no).
6. **Math Score** _(Integer)_ – Score in mathematics (0-100).
7. **Reading Score** _(Integer)_ – Score in reading (0-100).
8. **Writing Score** _(Integer)_ – Score in writing (0-100).


## **Objective of Analysis**
- Investigate the impact of **parental education and socio-economic factors** on student performance.
- Examine **gender differences** in academic scores.
- Analyse the effect of **test preparation courses** on student scores.
- Identify **correlations between math, reading, and writing performance**.


## **Potential Issues or Limitations**
- **Missing Data:** The dataset appears complete, but potential inconsistencies may exist in categorization.
- **Bias in Data:** The dataset groups students into predefined ethnic categories, which may not fully represent diversity.
- **Score Distribution:** Further analysis is required to detect any skewed distribution in scores.
- **Causal Limitations:** The dataset does not indicate causation, only correlations.


## **Research Questions to Address**
1. How does **parental education level** impact student scores?
2. Do students who **complete test preparation courses** perform better?
3. Is there a **gender disparity** in math, reading, and writing scores?
4. What is the correlation between math, reading, and writing scores?


## visualisation :
###  first visualisation : 
is the gender comparison to the math score

note : female scores were higher than male regards the reading score witch is 

did they finish the full 



![Screenshot 2025-02-14 183736.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/ug0qmENJhkQe5hk6jhU0M.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 183736.png")



### second visualisation :
the comparison is between the reading score compared to lunch 

what i saw is that student who payed "standereds" have got a higher reading score



![Screenshot 2025-02-14 184447.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/ZM9jrJZRdiG7Z3kq9d1b3.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 184447.png")



### third visualisation : 
this comparison is between writing score to test preparation and the classifier is the gender  

the females have completed the study preparation more compared to male 



![Screenshot 2025-02-14 185315.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/EJzIxBewOKmba9qCU8wma.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 185315.png")





## Data Cleaning :
data was clean there are no missing values so i have out lair attributes so they should be removed

before:



![image.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/BfVBVmabev4cyHs9YBBWp.png?ixlib=js-3.7.0 "image.png")



after :



![Screenshot 2025-02-14 190819.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/6MaEQGuq4meRXHDvubo5p.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 190819.png")



### rename values :
renaming the values because the names of the values were not understandable

before: 

![Screenshot 2025-02-14 191107.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/Y-ejGqB8Qb1g9WT1Q2PIN.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 191107.png")



after:



![Screenshot 2025-02-14 193132.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/DSdtbDSjCmT_G9wFTnWPF.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 193132.png")



before I start data mining transform data from numeric to nominal 

row 6 

### before :


![Screenshot 2025-02-14 193511.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/BzWFhU9SynN2EaiH3alXF.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 193511.png")



### after :


![Screenshot 2025-02-14 193828.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/gFDAUrYnDWDulxWfYfT9W.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 193828.png")



**Note : iv done the same for **column** 7 and 8 **

in number 7 I made the pins 3 pins for A grade in reading and b and c or below iv used the decreased filters



![Screenshot 2025-02-14 194858.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/xZlzT2SR6H4NaWXT9Jwcx.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 194858.png")



for column 8 :



![Screenshot 2025-02-14 195238.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/asJYNJBFyvpIDjOF59yFg.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 195238.png")



now we change the attributes names in maths to pass and fail 

![Screenshot 2025-02-14 195752.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/I_DQ9eSOwDzSjip_vue3c.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 195752.png")



now we rename the rest of the attributes

![Screenshot 2025-02-14 200301.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/41vSpOkFrM6JSRxoCQEjw.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 200301.png")



## Datamining :
### j48 tree:


![Screenshot 2025-02-14 200911.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/BdPMB4BbO_E6ZAnv9eedU.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 200911.png")



## J48 Decision Tree Analysis
**Overview:**
The J48 decision tree classifier was applied to the study performance dataset, which was split into 70% training and 30% testing data. Using Weka’s implementation, the algorithm constructs an interpretable tree by recursively splitting on key attributes, primarily academic scores, and refining decisions with demographic factors.

**Model Performance:**

- **Accuracy:** 93.33% (280 of 300 test instances correctly classified)
- **Kappa Statistic:** 0.5789 (moderate agreement beyond chance)
- **Error Metrics:**
    - **Mean Absolute Error:** 0.1215
    - **Root Mean Squared Error:** 0.241
    - **Relative Absolute Error:** 52.17%
    - **Root Relative Squared Error:** 82.37%
- **ROC Area:** 0.921 (excellent class discrimination)
**Key Observations:**

- The tree primarily utilizes academic performance attributes (math, reading, and writing scores) as decision nodes.
- Demographic factors such as gender and lunch type further refine the classification.
- The high accuracy and ROC Area validate the model’s effectiveness in predicting student performance.
**Interpretation:**
The J48 decision tree provides clear, actionable rules for classifying students. Its ability to effectively distinguish between passing and failing students underscores the importance of both academic indicators and demographic factors. These insights are valuable for developing strategies to enhance overall student performance.



## Aproiri :


![Screenshot 2025-02-14 202517.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/OhQ-3QRlBhhmWtHp-HlHh.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 202517.png")



## Association Rules Mining Analysis
**Overview:**
Association rules mining was applied to the study performance dataset (1,000 instances, 8 attributes) to uncover relationships between academic indicators. By setting a minimum support of 0.25 (i.e., the rule must cover at least 250 instances) and a minimum confidence of 0.9, we ensured that only robust and reliable rules were extracted.

**Algorithm Parameters:**

- **Minimum Support:** 0.25 (covering at least 250 instances)
- **Minimum Confidence:** 0.9 (rules must hold with at least 90% reliability)
- **Number of Iterations:** 15 cycles performed to generate frequent itemsets
**Frequent Itemsets Generated:**

- **L(1):** 15 single-item itemsets
- **L(2):** 20 two-item itemsets
- **L(3):** 6 three-item itemsets
**Key Association Rules:**

1. **Rule:** _writing_score = a_ → _math_score = pass_
    - **Confidence:** 100%
    - **Lift:** 1.18
_Interpretation:_ High writing scores (grade 'a') consistently predict a passing math score.
2. **Rule:** _reading_score = a_ → _math_score = pass_
    - **Confidence:** 100%
    - **Lift:** 1.18
_Interpretation:_ Top reading scores (grade 'a') guarantee a passing math score, indicating a strong association.
3. **Rule:** _reading_score = a AND writing_score = a_ → _math_score = pass_
    - **Confidence:** 100%
    - **Lift:** 1.18
_Interpretation:_ The combination of high reading and writing scores invariably leads to a passing math score.
Additional rules suggest that other factors—such as lunch status and test preparation course completion—also positively influence math performance, albeit with slightly lower confidence.

**Summary:**
The analysis reveals that exceptional performance in reading and writing is a robust indicator of passing math. The high confidence and lift values reinforce the reliability of these rules, highlighting the interdependence of academic performance metrics. These insights can be instrumental in devising strategies to enhance overall student achievement.



## SimpleKmeans : 


![Screenshot 2025-02-14 204315.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/p4_Lm5TTiMpA71CkI3uBQ.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 204315.png")



## Clustering Analysis: SimpleKMeans
**Overview:**
The SimpleKMeans algorithm was applied to the study performance dataset (1,000 instances, 8 attributes) to partition the data into 2 clusters based on Euclidean distance. Missing values were replaced with mean/mode values, and the model was built in 0.03 seconds.

**Model Details:**

- **Algorithm:** SimpleKMeans (weka.clusterers.SimpleKMeans)
- **Number of Clusters:** 2
- **Iterations:** 3
- **Within-Cluster Sum of Squared Errors:** 3233.0
**Final Cluster Centroids:**

**Cluster 0 (57% - 574 instances):**

- **Gender:** female
- **Race/Ethnicity:** group D
- **Parental Education:** some college
- **Lunch:** fullpay
- **Test Preparation:** none
- **Math Score:** pass
- **Reading Score:** a
- **Writing Score:** a
**Cluster 1 (43% - 426 instances):**

- **Gender:** male
- **Race/Ethnicity:** group C
- **Parental Education:** high school
- **Lunch:** fullpay
- **Test Preparation:** none
- **Math Score:** pass
- **Reading Score:** c
- **Writing Score:** c
**Interpretation:**
The clusters reveal distinct student profiles. Cluster 0 is dominated by female students with some college parental education and high reading/writing scores, whereas Cluster 1 primarily consists of male students with a high school background and lower reading/writing ratings. These groupings provide valuable insights into how demographic and academic factors align within the dataset.



## NaiveBayes :




![Screenshot 2025-02-14 204814.png](https://eraser.imgix.net/workspaces/d7z4aNmeFOUJPq6bbO7Q/3Tl3y7k0LGPg1Pb3jedwFSY7RAm1/gLfhoPg9EhXZqcxUt8zx-.png?ixlib=js-3.7.0 "Screenshot 2025-02-14 204814.png")



## Naive Bayes Classifier Analysis
### Overview
The Naive Bayes classifier (weka.classifiers.bayes.NaiveBayes) was applied to the study performance dataset, which contains 1,000 instances and 8 attributes. The model was trained on 70% of the data and evaluated on the remaining 30%, with both training and testing completing in approximately 0.01 seconds each.

### Model Performance
- **Accuracy:** 86% (258 out of 300 instances correctly classified)
- **Kappa Statistic:** 0.4581 (indicates moderate agreement beyond chance)
- **Error Metrics:**
    - **Mean Absolute Error (MAE):** 0.1435
    - **Root Mean Squared Error (RMSE):** 0.3027
    - **Relative Absolute Error:** 61.62%
    - **Root Relative Squared Error:** 103.43%
### Detailed Class Metrics
**For the 'fail' class:**

- **True Positive Rate (Recall):** 0.920
- **False Positive Rate:** 0.145
- **Precision:** 0.365
- **F-Measure:** 0.523
- **ROC Area:** 0.946
- **PRC Area:** 0.689
**For the 'pass' class:**

- **True Positive Rate (Recall):** 0.855
- **False Positive Rate:** 0.080
- **Precision:** 0.992
- **F-Measure:** 0.918
- **ROC Area:** 0.946
- **PRC Area:** 0.995
### Confusion Matrix
|  | **Predicted Fail** | **Predicted Pass** |
| ----- | ----- | ----- |
| **Actual Fail** | 23 | 2 |
| **Actual Pass** | 40 | 235 |
### Interpretation
The classifier exhibits robust performance, particularly in predicting the 'pass' class with exceptionally high precision (99.2%). Although the 'fail' class achieves a high recall (92%), its lower precision (36.5%) suggests some false positives. Overall, a ROC Area of 0.946 confirms that the Naive Bayes model effectively distinguishes between students who fail and pass.







