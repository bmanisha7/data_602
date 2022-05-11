### Abstract:
The primary goal of every construction permit is to guarantee that people are safe after the construction. We can avoid any accidents or concerns during the construction process while assuring the safety standards and the measures according to the place of the construction. The data which I have choosen is regarding the construction data from the Washington DC Construction permit dataset. The dataset consists information on requesting for an application for a permit in the Washington DC city from the year 2017 to 2021. I have checked the data across the time, trends, correlation between the variables using the matplotlib library. I have taken the status variable as a classification parameter. I wanted to create a model that predicts the issued label in order to identify the possibility of the application getting viewed and can be rejected before the officials make more efforts in viewing the application. I like to recognize the permits which are expected to be not issued.

### DataSet:
https://opendata.dc.gov/datasets/construction-permits-in-2020/explore?location=38.916593%2C-77.022175%2C11.73&showTable=true
Each record specifies a structure and allows information to be accessed through multiple features. The attributes include: X , Y, OBJECTID, APPLICATIONDATE, ISEXCAVATION, ISFIXTURE, ISPAVING,ISLANDSCAPING,ISPROJECTIONS,ISPSRENTAL ,TRACKINGNUMBER , PERMITNUMBER, INTAKEDATE, ISSUEDATE , EFFECTIVEDATE , EXPIRATIONDATE, XCOORD, YCOORD , STATUS, WLFULLADDRESS, PERMITTEENAME, OWNERNAME, CONTRACTORNAME, WORKDETAIL, READYFORREVIEWDATE, APPLICANTCOMPANYNAME, LATITUDE, LONGITUDE, GIS_ID, GLOBALID, CREATOR, CREATED, EDITOR,EDITED.

The columns which I have worked on are:

**STATUS:** This columns tells about the permit status, 

**APPLICATIONDATE:** This attribute explains the applied form for the permit, 

**PERMITTEENAME:** This column tells which permittee gives the permits for construction, 

**OWNERNAME:** It explains about the owners of the construction permits, 

**APPLICATIONCOMPANYNAME:** This gives information regarding which company has applied for permit.

### EDA:
I have checked the data and removed the unwanted values and the unique values. I have grouped the status column values into few categories like ‘Cancel/Withdrawn’, ‘Revise/Resubmit’, ‘Denied’, ’Suspended’, ‘Revoked’ into Not issued and Approved into Issued. Then using the status values I have visualized few of the values and in which years do the construction permits are high. Plotting the top companies and permittees for the applications. From the graphs I have observed there are more permits in the year 2020 and there are also more permits which are not issued than 2019.

### Future Performance:
As mentioned in the abstract I like to predict the permits which can be issued or not. Based on this dataset I like to work on few models which will help me to predict the problem and provide me certains results according to the conditions.

### Data Cleaning
After observering from the EDA I have dropped few columns and used the attributes which are helpful for the modeling.

### Feature Engineering
I have used One hot encoding(OHE) which is a popular technique used for categorical encoding. With the help of simple imputer the pipeline managed handling the missing data. 

### Modeling
Independent variables are analyzed to determine the binary outcome with the results falling into one of two categories. The independent variables can be categorical or numeric, but the dependent variable is always categorical in case of classification algorithms. I have used logistic regression model , Decision trees, support vector classifer and neural networks. Parameters are tuned using grid search for the Machine learning models. 

### Results and Discussions
Logistic Regression score:0.7753533283093608 <br />
Decision Tree score:0.844604552800145 <br />
Support Vector Classifier score:0.8308271012657477 <br />
Neural Network score:0.861576660459342 <br />

Logistic: ROC AUC=0.7703 <br />
Tree: ROC AUC=0.8307 <br />
SVC: ROC AUC=0.8158 <br />
Neural Network: ROC AUC=0.8457 <br />

Regarding ROC AUC score , Decision tree and Neural network is more than other algorithms. Accuracy is better for Neural Network and Tree. Rather than the machine learning algorithms, Neural Network performed better according to this data.

### Next steps
Working with more features can help us in understanding the data more. <br />
Applying other parameters improves the models performance. <br />
Instead of just predicting two labels Issued and Not issued, we can predict more specific other classes. <br />

### References
https://github.com/appliedecon/data602-lectures

https://www.statology.org/plot-multiple-roc-curves-python/
