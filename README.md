[![Rawsec's CyberSecurity Inventory](https://inventory.raw.pm/img/badges/Rawsec-inventoried-FF5050_flat.svg)](https://inventory.raw.pm/ctf_platforms.html#miniCTF)

# MINICTF

### A platform build in django for hosting CTF events. 

#### Live demo 

[https://xyz-minictf.herokuapp.com/](https://xyz-minictf.herokuapp.com/)

#### FEATURES :

* Cool Interface
* Score Board
* Responsive Design
* Password Change Support 
* Discussion Forums
* and a lot more.

#### SCREENSHOTS :

Challenge Page

<img src="readmeimg/challenges.png" width="100%">

Challenge View

<img src="readmeimg/onechallenge.png" width="100%">

Score Board

<img src="readmeimg/scoreboard.png" width="100%">

Team Details

<img src="readmeimg/teams.png" width="100%">

Discussion Forums

<img src="readmeimg/forum.png" width="100%">


#### Dev env setup

##### Requirments

> Rename .env.example to .env and change the value of KEY. 
>
> **Note**: Keep this value a secret.

###### Docker Setup

```bash
  make docker_build
  make docker_run
```

This will start the server at port 8000.

###### Local Setup

```
python 3.x
django 2.0
```

Install [Pipenv](https://pypi.org/project/pipenv/)

<b>Want to make this process fast. Switch to [local branch](https://github.com/DivyanshuSahu/miniCTF/tree/local)</b>

###### Install miniCTF

```bash
  git clone https://github.com/DivyanshuSahu/miniCTF.git
  pipenv shell
  pipenv install
  python manage.py makemigrations accounts challenges forums
  python manage.py migrate
  python manage.py runserver
```

Then register or create superuser and add challenges.
