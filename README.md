# Health Insurance Cross Sell

# 1. Business Problem.
A company that traditionally provides Health Insurance intends to offer its customers a new product, a Vehicle Insurance. In order to achieve this purpose efficiently, With limited resources to contact potential customers interested in purchasing the product, it is necessary to build a ranking of customers to improve the performance of adherence to the product. This is a classification project (Learning to Rank).

# 2. Business Assumptions.

The Marketing Manager stated that they there is a limited budget for prospecting customers. Therefore, the company wants to obtain an ordered list of customers most likely to purchase vehicle insurance to maximize customer conversion.

# 3. Solution Strategy

My strategy to solve this challenge was: The method applied was CRISP-DM:

**Step 01. Data Description:** The objective is to use statistical metrics to identify outliers in the business scope.

**Step 02. Feature Engineering:** Derive new attributes based on the original variables to better describe the phenomenon to be modeled.

**Step 03. Data Filtering:** Filter rows and select columns that do not contain information for modeling or do not correspond to the business scope.

**Step 04. Exploratory Data Analysis:** Explore the data to find insights and better understand the impact of variables on model learning.

**Step 05. Data Preparation:** Prepare data so machine learning models can learn specific behavior.

**Step 06. Feature Selection:** Selection of the most significant attributes to train the model.

**Step 07. Machine Learning Modelling:** machine learning model training

**Step 08. Hyperparameter Fine Tunning:** Choose the best values for each of the parameters of the model selected in the previous step.

**Step 09. Convert Model Performance to Business Values:** Convert model performance to a business result.

**Step 10. Deploy Modelo to Production:** Publish the model to a cloud environment so that other people or services can use the results to improve the business decision.

**Step 11. Google Sheets:** Creation of google sheets button to show custumer score.

# 4. Top 3 Data Insights

**H2.** Clientes com carros novos/seminovos, tem mais interesse em seguro de veículos. **True Hypothesys**
<div align="">
<img src="https://user-images.githubusercontent.com/94291995/168711521-a080a4d9-6db9-46a4-ac2f-381362ad9dfd.png" />
</div>

**H3.** Clientes acima de 30 anos são mais interessados em adquirir seguro de veículos. **True Hypothesys**

<div align="">
<img src="https://user-images.githubusercontent.com/94291995/168711688-816b2185-1dd6-480f-9899-a3374f9c7e40.png" />
</div>

**H5.** Mulheres tem mais eventos de dano a veículos, do que homens. **False Hypothesys**

<div align="">
<img src="https://user-images.githubusercontent.com/94291995/168711733-41835a95-bba9-4c9a-9148-5bf467110d23.png" />
</div>


# 5. Machine Learning Model Applied

KNN Classifier

Logistic Regression

Random Forest Classifier

LGBM Classifier

# 6. Machine Learning Modelo Performance

<div align="">
<img src="https://user-images.githubusercontent.com/94291995/168709406-3c62214b-a409-419d-a77d-988d4d6da296.png" />
</div>

- The precision@k is the proportion of recommended items in the top-k set that are relevant, where k is the number (or percentage, in this case) of rows of the class 1 (those that are intereseted in vehicle insurance) in the sorted probability table.
    
- The recall@k is the proportion of relevant items found in the top-k recommendations.

<div align="">
<img src="https://user-images.githubusercontent.com/94291995/168710206-baa76e5c-06e3-4807-94a8-c3ff804d1659.png" />
</div>


# 7. Business Results

We can note that by applying this model approximately 93% of potential customers interested in vehicular insurance will be converted by addressing 40% of the total customers currently with only health insurance.

The model was deployed on Heroku and available through a spreadsheet in Google Sheets  (https://docs.google.com/spreadsheets/d/1SQx0MADjfRLo49gcAw0k8UXndCSEPEBxxnJCOJvNn9Q/edit#gid=0)

<div align="center">
<img src="https://user-images.githubusercontent.com/94291995/168708505-c90edd94-d887-4047-b136-a3ac43cec75f.png" />
</div>

# 8. Conclusions

With the use of the model in production, it is expected, at least, to double the efficiency in the acquisition of new clients for vehicle insurance.

This is because you will only need to contact 40% of customers to get over 90% conversion. Without the model, when contacting purely random customers, it is reasonable to say that to have 90% of customers likely to close a deal, you would also have to contact 90% of the total list.


# 9. Next stepsPossible points to be addressed in the second cycle:

- Work with new combinations of feature

- Test new machine learning models

- Try new models after balance

- Apply cross validation and hyper paramaters

# 10. Technologies

- Jupyter;
- AWS;
- Postgres;
- Python.
