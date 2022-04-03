# handm_data_visualize_app
Data visualization app for H&amp;M competition in kaggle by streamlit.
 
competition page: https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/

## Features 


https://user-images.githubusercontent.com/43205304/161410926-0dc5929f-cc9c-4e93-ba77-5ca420e73f5c.mov



## Directory
```
.
├── README.md
├── app.py
├── config.yaml
├── data (competition dataset folder)
└── requirements.txt
```


## Environment setup
Here I show how to build an environment.
If you already have the competition project, simply prepare `app.py` and `config.yaml` in your project and set the data path in `config.yaml`.

1. Clone this repository
```
git clone https://github.com/kuto5046/handm_data_visualize_app.git
```

2. Make environment

First, create your favorite virtual development environment.(docker, venv, poetry etc...)

Then, run this command to install necessary libraries in your environment.
```shell
pip install -r requirements.txt
```

3. Prepare data 

Prepare competition data in `data` folder.
I show an example of using the `kaggle api`, but you can also download it manually.
```
cd data
kaggle competitions download -c h-and-m-personalized-fashion-recommendations
unzip h-and-m-personalized-fashion-recommendations.zip
```

## Usage
run in your terminal this command
```shell
streamlit run app.py
```
Then connect to the output URL or `localhost:8501`
