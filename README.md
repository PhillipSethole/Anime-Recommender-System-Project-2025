# Anime Recommender System

<div id="main image" align="center">
  <img src="https://mostaql.hsoubcdn.com/uploads/thumbnails/1450164/661a5b0c8a072/dataset-card.jpg" width="550" height="300" alt=""/>
</div>

## Table of contents
* [1. Project Overview](#project-description)
* [2. Dataset](#dataset)
* [3. Packages](#packages)
* [4. Environment](#environment)
* [5. MLFlow](#mlflow)
* [6. Streamlit](#streamlit)
* [7. Team Members](#team-members)

## 📌1. Project Overview <a class="anchor" id="packages"></a>
This project builds a smart anime recommendation system that helps users discover new anime based on their preferences. The system uses **collaborative filtering** and **content-based filtering** to generate personalized recommendations. By analyzing user ratings and anime details, it suggests relevant anime while improving accuracy through model tuning and evaluation.


## 2. Dataset <a class="anchor" id="dataset"></a>
The project uses three datasets:

The dataset is comprised of Anime content that is needed for a recommender system and the categories are based on `ID`, `name`, `genre`, `type`, `episodes` and `ratings`. You can find both the `train.csv` and `test.csv` datasets 


## Dataset Features

### 1. Anime Dataset  

| **Columns**   | **Description**  |  
|--------------|-----------------|  
| `anime_id`   | myanimelist.net's unique ID identifying an anime. |  
| `name`       | Full name of the anime. |  
| `genre`      | Comma-separated list of genres for this anime. |  
| `type`       | Movie, TV, OVA, etc. |  
| `episodes`   | The number of episodes in the series (1 if movie). |  
| `rating`     | Average rating out of 10 for this anime. |  
| `members`    | Number of community members in this anime's "group". |  

### 2. Train Dataset  

| **Columns**   | **Description**  |  
|--------------|-----------------|  
| `user_id`    | Non-identifiable randomly generated user ID. |  
| `anime_id`   | The anime that this user has rated. |  
| `rating`     | Rating out of 10 assigned by the user (-1 if the user watched it but didn't assign a rating). |  

### 3. Test Dataset  

| **Columns**   | **Description**  |  
|--------------|-----------------|  
| `user_id`    | Non-identifiable randomly generated user ID. |  
| `anime_id`   | The anime that this user has rated. |  


## 3. Packages <a class="anchor" id="packages"></a>

To carry out all the objectives for this repo, the following necessary dependencies were loaded:
+ `Pandas 2.2.2`, `Numpy 1.26` and `json `
+ `Matplotlib 3.8.4` and `seaborn `
+ `sklearn.model_selection` and `nltk`
+ `scikit-learn all sklearn`
+ `mlflow `and `pickle`
+ `re` and `html`
+ `time` and `operator`
+ `scikeras`
+ `scipy`
+ `surprise`
+ `tensorflow`
+ `streamlit`


## 4. Environment <a class="anchor" id="environment"></a>

It's highly recommended to use a virtual environment for your projects, there are many ways to do this; we've outlined one such method below. Make sure to regularly update this section. This way, anyone who clones your repository will know exactly what steps to follow to prepare the necessary environment. The instructions provided here should enable a person to clone your repo and quickly get started.

### Create the new evironment - you only need to do this once

```bash
# create the conda environment
conda create --name <env>
```

### This is how you activate the virtual environment in a terminal and install the project dependencies

```bash
# activate the virtual environment
conda activate <env>
# install the pip package
conda install pip
# install the requirements for this project
pip install -r requirements.txt
```

## 5. MLFlow<a class="anchor" id="mlflow"></a>

MLflow is used for tracking experiments, hyperparameter tuning, and managing different model versions. It helps compare different configurations to select the best-performing recommendation model.

- Follow the official MLflow setup guide: https://www.mlflow.org/docs/latest/quickstart.html

## 6. Streamlit<a class="anchor" id="streamlit"></a>

### What is Streamlit?

[Streamlit](https://www.streamlit.io/)  is a framework that acts as a web server with dynamic visuals, multiple responsive pages, and robust deployment of your models.

In its own words:
> Streamlit ... is the easiest way for data scientists and machine learning engineers to create beautiful, performant apps in only a few hours!  All in pure Python. All for free.

> It’s a simple and powerful app model that lets you build rich UIs incredibly quickly.

[Streamlit](https://www.streamlit.io/)  takes away much of the background work needed in order to get a platform which can deploy your models to clients and end users. Meaning that you get to focus on the important stuff (related to the data), and can largely ignore the rest. This will allow you to become a lot more productive.  

##### Description of files

For this repository, we are only concerned with a single file:

| File Name              | Description                       |
| :--------------------- | :--------------------             |
| `base_app.py`          | Streamlit application definition. |


#### 6.1 Running the Streamlit web app on your local machine

As a first step to becoming familiar with our web app's functioning, we recommend setting up a running instance on your own local machine. To do this, follow the steps below by running the given commands within a Git bash (Windows), or terminal (Mac/Linux):

- Ensure that you have the prerequisite Python libraries installed on your local machine:

 ```bash
 pip install -U streamlit numpy pandas scikit-learn
 ```

- Navigate to the base of your repo where your base_app.py is stored, and start the Streamlit app.

 ```bash
 cd Amime_Recommender_system/Streamlit/
 streamlit run base_app.py
 ```

 If the web server was able to initialise successfully, the following message should be displayed within your bash/terminal session:

```
  You can now view your Streamlit app in your browser.

    Local URL: http://localhost:8501 
    Network URL: http://192.168.43.41:8501
```
You should also be automatically directed to the base page of your web app. This should look something like:

<div id="s_image" align="center">
  <img src=""C:\Users\lebog\Documents\Team 2 Anime recommender system\Anime-Recommender-System-Project-2025\anime app screenshot.png"" width="850" height="400" alt=""/>
</div>

Congratulations! You've now officially deployed your first web application!

#### 6.2 Deploying your Streamlit web app

- To deploy your app for all to see, click on `deploy`.
  
- Please note: If it's your first time deploying it will redirect you to set up an account first. Please follow the instructions.

## 7. Team Members<a class="anchor" id="team-members"></a>

| Name                                                                                        |  Email              
|---------------------------------------------------------------------------------------------|--------------------             
|[Nombulelo Perfidia Tracy Nyoni]                                                             |	nombulelotracy@gmail.com
|[Phillip	Sethole]                                                                            |	philipsethole346@gmail.com
|[Sanele Bhembe] 	                                                                            | sanelebhembe12@gmail.com
|[Fransisca Matlou Nong]	                                                                    | matlou9637@gmail.com
|Mzwandile Stuurman]	                                                                        | stuurmanmzwandile@gmail.com
|[Lebogang Swaratlhe]	                                                                        | lebogangswaratlhe@gmail.com

