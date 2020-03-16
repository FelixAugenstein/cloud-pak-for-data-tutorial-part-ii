<h1 align="center" style="border-bottom: none;">:bar_chart: IBM Digital Tech Tutorial: Watson Studio Part II</h1>
<h3 align="center">In this hands-on tutorial you will build and evaluate machine learning models by using the AutoAI feature in IBM Watson Studio.</h3>

## Prerequisites

1. Sign up for an [IBM Cloud account](https://cloud.ibm.com/registration).
2. Fill in the required information and press the „Create Account“ button.
3. After you submit your registration, you will receive an e-mail from the IBM Cloud team with details about your account. In this e-mail, you will need to click the link provided to confirm your registration.
4. Now you should be able to login to your new IBM Cloud account ;-)

## Digital Tech Tutorial Watson Studio Part I to IV

This tutorial consists of 4 parts, you can start with part I or any other part, however, the necessary environment is set up in part I.<br>
[Part I - data visualization, preparation, and transformation](https://github.com/FelixAugenstein/digital-tech-tutorial-watson-studio)<br>
[Part II - build and evaluate machine learning models by using the AutoAI](https://github.com/FelixAugenstein/digital-tech-tutorial-watson-studio-part-ii/)<br>
[Part III](https://github.com/FelixAugenstein/digital-tech-tutorial-watson-studio-part-iii/)<br>
[Part IV](https://github.com/FelixAugenstein/digital-tech-tutorial-watson-studio-part-iv/)

The 4 parts of this tutorial are based on the [Learning path: Getting started with Watson Studio](https://developer.ibm.com/series/learning-path-watson-studio/).

## Create a new AutoAI model

1. Select the Assets tab for your Watson Studio project.
2. In the Asset tab, click the Add to Project command.

![Auto AI Project](readme_images/auto-ai-project.png)

3. Select the AutoAI Experiment asset type.
4. In the Create an AutoAI experiment window:

- Select From Blank as the experiment type.
- Enter an Asset Name, such as ‘customer-churn-manual’.
- For the Machine Learning Service, select the Watson Machine Learning service that you previously created for the project. If you have not created one, please do so now. It is available in the IBM Cloud Catalog under the category AI.
- Then click Create.

![Create Experiment](readme_images/create-experiment.png)

5. In the Add training data window:

- Click Select from project.
- Select the Kaggle data asset previously added to the project (e.g. customer-churn-analysis, don't select any shaped data assets).
- Click Select Asset.

![Select from Project](readme_images/select-from-project.png)

## Run and train the model

From the Configure AutoAI experiment window:

1. In the Select column to predict box, select churn.

![Select Prediction Column](readme_images/prediction-column.png)

2. Keep the default prediction type of Binary Classification, and the optimized metric of ROC AUC (Receiver Operating Characteristics / Area Under Curve).
3. Click Run experiment.

As the experiment is run, you see the different pipelines in the relationship map. After it finishes, a list of completed models is listed at the bottom of the panel, in order of accuracy. You can take a look at the Pipeline comparison or the Progress map, by clicking swap view.

![Pipelines](readme_images/pipelines.png)

For our data, Pipeline 4 was ranked the highest, based on our “Area under the ROC Curve” (ROC AUC) metric. After the AutoAI experiment completes, it is saved in the Watson Studio project. You can view it from the Assets tab under AutoAI experiments.

## Evaluate the model performance

On the AutoAI Experiment page, there are a number of options available to get more details on how each pipeline performed.

## Deploy and test the model using Watson Machine Learning service

text

## If you have any questions just contact me

Felix Augenstein<br>
Digital Tech Ecosystem & Developer Representative @IBM<br>
Twitter: [@F_Augenstein](https://twitter.com/F_Augenstein)<br>
LinkedIn: [linkedin.com/in/felixaugenstein](https://www.linkedin.com/in/felixaugenstein/)
