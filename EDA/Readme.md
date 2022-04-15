### Abstract:
The primary goal of every construction permit is to guarantee that people are safe after the construction. We can avoid any accidents or concerns during the construction process while assuring the safety standards and the measures according to the place of the construction. The data which I have choosen if regarding the construction data from the Washington DC Construction permit dataset. The dataset consists information on requesting for an application for a permit in the Washington DC city from the year 2017 to 2021. I have checked the data across the time, trends, correlation between the variables using the matplotlib library. I have taken the status variable as a classification parameter. I wanted to create a model that predicts the issued label in order to identify the possibility of the application getting viewed and can be rejected before the officials make more efforts in viewing the application. I like to recognize the permits which are expected to be not issued.

### DataSet:
https://opendata.dc.gov/datasets/construction-permits-in-2020/explore?location=38.916593%2C-77.022175%2C11.73&showTable=true
Every record identifies a construction permits information using various features. The attributes include: X , Y, OBJECTID, APPLICATIONDATE, ISEXCAVATION, ISFIXTURE, ISPAVING,ISLANDSCAPING,ISPROJECTIONS,ISPSRENTAL ,TRACKINGNUMBER , PERMITNUMBER, INTAKEDATE, ISSUEDATE , EFFECTIVEDATE , EXPIRATIONDATE, XCOORD, YCOORD , STATUS, WLFULLADDRESS, PERMITTEENAME, OWNERNAME, CONTRACTORNAME, WORKDETAIL, READYFORREVIEWDATE, APPLICANTCOMPANYNAME, LATITUDE, LONGITUDE, GIS_ID, GLOBALID, CREATOR, CREATED, EDITOR,EDITED.

### EDA:
I have checked the data and removed the unwanted values and the unique values. I have grouped the status column values into few categories like ‘Cancel/Withdrawn’, ‘Revise/Resubmit’, ‘Denied’, ’Suspended’, ‘Revoked’ into Not issued and Approved into Issued. Then using the status values I have visulaized few of the values and the in which years do the construction permits are high.

### Future Performance:
As mentioned in the abstract I like to predict the permits which can be issued or not. Based on this problem I like to work on few models which will help me to predict the problem and provide me certains results according to the cinditions.
