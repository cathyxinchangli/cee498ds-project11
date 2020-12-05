# Linear regression model
This section will cover how a linear regression model was constructed in order to predict household energy consumption, as well as discuss the limitations of a linear model. 

### Data preparation
As it has been described in previous sections, the data used for this Kaggle competition came in three different files: train data, building metadata and weather train data. 
Since the dataset contains over 20 million readings and numerous features, issues with RAM usage had to be dealt with. The main problem was that not all desirable features could 
be included in the before RAM usage hit the limit. 

### Kaggle Score
The best public score (RMSLE) that could be obtained with this linear model was 4,5.

### Imporvements
Is RMSLE of 4,5 the limit for linear regression? Most likely not. In the model and data preparation, several things can be made better. First, the datasets can be optimized even better. Site_id 13 was removed because the values were suspiciously high, as seen in the EDA. In this case, an even more in-depth "cleaning" can be made and locade the exact building_id (or several building_ids) that is responsible for the data anomaly. This deeper cleaning was made for the other models, but not for the linear regression model.
Furthermore, if cateorical values could be implemented not only in the training, but also the prediction, perhaps a better score could be obtained. However, it must be realized that no matter how many parameters are added to a linear model, it will still only predict new values linearly. If many or strong non-linear relationships exist between the target variable and predition features, a linear model will never be able to perform nearly as good as e.g. neural networks.
