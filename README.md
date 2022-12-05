# ML for Material Science

## Introduction
This machine learning is one of the example of the utilization of ML in material science regime.
The purpose is to predict the superconductivity temperature of material, especially, known-as conventional superconductor.
Superconductor is a set of physical properties observed in certain materials where electrical resistance vanishes and magnetic flux fields are expelled from the material. This materials have various functionalities for instance, magnetic levitation train, quantum computers, etc.

## Method
### Dataset
The dataset itself was extracted from NIMS Database (https://dice.nims.go.jp/news/2021/12/20211221.html).
The daset consists of chemical compound and Tc (Temperature when the material start behaving as superconductor)
### Data Cleansing
To provide the realistic dataset, I ignore empty data and purposely remove debatable materials, known-as unconvetional superconductor (Fe, Cu, Mn, etc).
### Machine Learning
As the example, I used random forest regression to predict the Tc of materials, This method had been studied by Stanev, et.al (https://www.nature.com/articles/s41524-018-0085-8) and confirmed the accuracy.

## Result
The result is visualized in graph (x-y axis), x-axis refers measured Tc (based on dataset) while y-axis is predicted Tc (based on ML) respectively. 
<br>
From the prediction, the $R^{2}$ of both train and test data rae more the 90%, which indicates the prediction is fairly in good aggreement with experiemnt $T_{c}$
<br>
<br>
<img width="624" alt="image" src="https://user-images.githubusercontent.com/26571248/205536262-3b7029bc-cd3a-4ce9-beb0-d771c8966952.png">


