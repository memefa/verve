# verve

1. Identified potential problems that might make building a classification model difficult are:

--The first problem is the unbalance number of records for the class of gender: 2663 for male vs 1037 for female.

--The second problem is value missing for device_name that is megarity of records and better to be removed of features for making a classification model.

--The third problem is being meaningless of device_name feature that could not be used as an efficient feature unless used by feature engineering methods 
  like NLP for detection of names related to genders and making a better feature value.

--The forth problem could be NAN values of app_category feature and the related records should be removed.

--The fifth problem could be NAN values of ad_category feature and the related records should be removed.

--The sixth problem could be click feature which has the varience of about zero and should be removed from features.
   



2. The best features have low corrolation with each other and high corrolation with target variable and reasonable variance to make good relationship with target variable. Also, there      are some feature selection and feature engineering methods to choose best features or transform feature vector to a new one with lower dimension and higher quality. 

--The recommended features for making a model for classification are: {app_category, ad_category, interaction_with_app}




3. Regarding statistics of features specially the gender variable with different number of samples per class, the proposed classification method that is not sensitive much for unbalance    number of data for classes is random forest which is combination of several decision trees and is useful for gategorical and low number of features but has some weaknesses about real    values however, XGBoost algorithm recently yields to top accuracy in many problems!!!

