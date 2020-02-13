# Video Analysis

## Setup

The first thing to do is to download the project and set the current directory to project:

download link : https://drive.google.com/drive/folders/17J9auYwmUEK3dl6Y4Ntcsjpf8IwIVkqm

```sh
$ cd Django_ML
```

Create a virtual environment to install dependencies in and activate it:

MacOs:

```sh
$ virtualenv --no-site-packages env
$ source env/bin/activate
```
Windows:
```sh
$ virtualenv --no-site-packages env
$ env/Scripts/activate
```

Then install the dependencies:

```sh
(env)$ pip install -r requirements.txt
```
Note the `(env)` in front of the prompt. This indicates that this terminal
session operates in a virtual environment set up by `virtualenv`.

Once `pip` has finished downloading the dependencies:
```sh
(env)$ cd website
(env)$ python manage.py migrate
(env)$ python manage.py runserver
```
And navigate to `http://127.0.0.1:8000/`.

## Walkthrough

>The website consists of a search page, subsequent search result page and an analysis page.

>In order to search, enter the desired objects, text or person you want to see in a video.( To enter a value press TAB).On completion, you will receive a search result. 

>The video display page consists of a personalised bio of each person detected by the facial recognition algorithm and also a chart indicating the similarity between the search and the chosen result.

>The analysis page shows statistics of the number of videos watched by a person in the last 5 months, distribution of most watched objects and faces, and also personalised suggestions based on search history.
