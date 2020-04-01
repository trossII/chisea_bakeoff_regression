# Bake off challenge: Regression

![bakeoff](https://media.giphy.com/media/WvRgv9DdgJtPcIlTEI/giphy.gif)

For this challenge, we will throw you back into the familiar territory of  regression, and give you what will (most likely) be your first exposure in a Kaggle-like "contest."  Given a dataset of house prices in King County, Washington, you will be tasked with fitting a model on a labeled training dateset, and submitting housing price predictions on an unlabeled test dataset.  Don't worry if you've already seen this dataset; remember reiteration is a crucial component of CRISP-DM.  Have fun with this. 

## Data files

You will find two data files in this repo, along with one file describing the features.

1. `kc_house_data_train.csv`
> Labeled training data to train your model on.  Target variable is the continuous feature 'price'

2. `kc_house_data_test_features.csv`
> An unlabeled set of test features.  The columns match the train set, but the 'price' column is missing. Take your fit your model on the training data, then use that fit object to make predictions on the test features dataset.

3. `feature_descriptions.md`
> A description of features that apply to both train and test sets.


## Instructions
- Every team member fork and then clone this repo onto your computer. Figure out a strategy for how to collaborate, which may look like selecting one team member as the primary "coder".  We leave it to you to set-up a productive team dynamic, but keep in mind, the deliverable of this exercise is one csv file.   
- Load up a Jupyter and start CRISP'ing.
- The instructions for this bakeoff are limited with regards to modeling. Go wild. Use any model you want.  Feature engineer your head off.
- Once you are satisfied with your model, or you find time running out, use the `kc_house_data_test.csv` to predict a price for each of the 4323 house records.  See Submission guidelines below. 
- Please be sure to use your own work.  If you have worked on this dataset before, don't copy and paste your previous work. Obviously there is no way that we can ask you not to use past experience, but we can ask you not to use past code.

## Submissions
Save your predictions in a csv file with the following pattern. 
- `housing_preds_yourteaminitials.csv`
- For example, if Brian and Erin were a team, their submission would look like `housing_preds_bmeh.csv`

- There are different ways to turn arrays to csv's.  You can use any method you choose, but be sure your submission has no heading, no index and one column. Your submission must match the number of records in the `kc_house_data_test_features.csv`. Don't worry about rounding.  A valid submission could look like below. 

401412.6923102136<br>
501023.6923102136<br>
310304.62734089<br>
1030130.2812897698<br>
...

- Please no header on your csv submission.

- You will be given **3 hours** to build your best model using the training data. There is a hard cuttoff at 3 hours. Any late submissions will not be considered. 
- Slack your csv file to the `seattle-chicago-ds-012720` channel before time is up. Any submissions after the 3 hour deadline will be evaluated, but not included in the judging. (Chicago will start sooner and have an earlier submission deadline than Seattle this time around.)

## Metrics
Test results will be scored by RMSE. The group which submitted the predictions with the lowest RMSE will be anounced Thursday morning. As reward, they will receive bragging rights that span from the Midwest to the Pacific coast.

## Lastly
- After submission, push your repo with your work to your forked repo. In this way, your peers will be able to gain valuable wisdom from the different tactics employed.
