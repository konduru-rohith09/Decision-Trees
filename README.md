# Decision Tree Classifier - Play Tennis Example

This project demonstrates a **Decision Tree Classifier** to predict whether people will play tennis based on the weather. It’s a small dataset, ideal for learning how decision trees work.

## 1. The Dataset

We have 8 samples with 4 features:

 **Outlook:** Sunny, Overcast, Rain  
 **Temperature:** Hot, Mild, Cool  
 **Humidity:** High, Normal  
 **Wind:** Weak, Strong  

The target is **PlayTennis** (Yes/No).  

It answers questions like:  
* If it’s Sunny, Hot, and Humid with Weak wind, will we play tennis?



## 2. Encode Categorical Data

Machine learning models cannot work with text directly, so we convert categories into numbers using `LabelEncoder`.  

* Example: `Sunny → 2, Overcast → 0, Rain → 1`  

This prepares the dataset for training.



## 3. Features & Target

We separate the **features (`X`)** and the **target (`y`)**:

* `X` → all input columns
 * `y` → what we want to predict (`PlayTennis`)



## 4. Train the Decision Tree

We create a **Decision Tree Classifier** using the **entropy** criterion:
* Entropy helps the tree decide the best feature to split at each step.  
*  The model learns rules like: “If Outlook = Rain and Wind = Weak → PlayTennis = Yes”.



## 5. Visualize the Tree

We can plot the tree to see the splits and decisions:

* Each node shows a feature and condition.  
* Leaves show predicted class (Yes/No).  
* Colors indicate class distribution, making it easy to interpret.



## Key Learnings

* Decision Trees are simple, intuitive, and easy to visualize.  
* Label encoding is essential for categorical data.  
* Even small datasets can help understand machine learning concepts.



## Requirements

* Python 3  
* pandas  
* scikit-learn  
 * matplotlib
