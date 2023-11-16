# Modelling-Cement-Production

Cement strength is essential in production ,to get cement strenght we combine different materials.Cement is manufactured in a rather complex process with a variety of ingredients, which is why testing is essential in ensuring that the specifications and regulations can be met. Cement plays a critical  role in the mixture of concrete and mortar, and so it has be of high quality. 
Concrete is one of the main materials in many building projects. It is a material we need to know a lot about.Testing concrete is not complicated but does involve a number of different tests to establish the working parameters of the cement.Now, this is where concrete shines. Concrete and mortar can withstand high compressive loads in part due to the cement used in the mixture. The performance of concrete under compressive loads is influenced by the cement used.

Cement paste strength is typically defined in three ways: compressive, tensile and flexural. These strengths can be affected by a number of items including: water-cement ratio, cement-fine aggregate ratio, type and grading of fine aggregate, manner of mixing and molding specimens, curing conditions, size and shape of specimen, moisture content at time of test, loading conditions and age.

For this project I used Compressive paste  strenght .The compressive strength of the concrete cube test provides an idea about all the characteristics of concrete. By this single test one judge that whether Concreting has been done properly or not.The idea was to use Regression to predict  the compressive strenght based on various materials such as Blast Furnace Slag,Water ,Ash and Age among others.

Regression is a statistical method where we try to find a linear relationship between variable ,after finding the linear relationship we create a model
which we use as our predictor model.

I first imported my dependencies and loaded my dataset 
![Introduction](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/a956ec83-0c9b-4996-9564-115b0ed806e4)

The next step was to find out basic statistical information :

![Describe](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/a1dec766-686d-436e-a620-5a285e006944)

After knowing the statistical information ,I proceeded to data analaysis. To work faster I created a custom function to avoid repetition of code ,then uses Python loop to iterate through my columns 

![Custom Function and EDA](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/3abaac6b-2b77-468e-8563-632f7249a091)

Here is the EDA in action , a histogram .For histograms we deal with univariate data where we use the frequency of one variable as a measure 

![Eda in Action](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/75b5ab30-3941-4964-860f-3f1735939c3c)

Heres the distribution of Coarse aggregate distribution :

![Eda in action 2](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/7a508b80-1b60-4b01-ad3e-1ee96342d8c2)\

 Correlations are really important in Regression ,choosing  highly correlated variables ensures that we come up a good model.

 ![Getting correlation](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/2db8099f-1ea9-44c1-8064-134577419a68)

I created a heatmap to clearly show my correlations

![Correlation Heatmap](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/b085c727-3ecd-49f6-b537-c31ba2974cb9)

Before feeding data into our machine learning model we are supposed to choose the feature and target variables which I did . I then proceeded to scale my data ,to improve model efficiency

![Train test split and scaling data](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/e5f0583e-f49d-43e7-a321-46b738cc6551)

 I chose Linear Regression and XGBoost Regression as my machine learning models.XGBoost stands for Extreme Gradient Boosting, is a gradient-boosted decision tree (GBDT) machine learning library. It provides parallel tree boosting and is the leading machine learning library for regression.
 
 ![Machine Learning](https://github.com/muyale/Modelling-Cement-Production/assets/111242297/68840541-a514-40da-b142-9bac44efbfab)

#Conclusion 

XGBoost outperformed ordinary Linear Regression and is hence the best one to predict cement strenght .






 REFERENCES 
 
 https://pavementinteractive.org/reference-desk/materials/portland-cement/portland-cement-strength/
 https://reinforcingsteelcontractors.co.za/cement-strength-classes-and-what-they-mean/
