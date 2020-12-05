# Linear regression model
This section will cover how a linear regression model can be constructed in order to predict household energy consumption, as well as discuss the limitations of a linear model. 

### Data preparation
As it has been described in previous sections, the data used for this Kaggle competition came in three different files: train data, building metadata and weather train data. 
Since the dataset contains over 20 million readings and numerous features, issues with RAM usage had to be dealt with. The main problem was that not all desirable features could 
be included in the before RAM usage hit the limit. 
