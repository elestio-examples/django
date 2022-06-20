# Django on Elestio

This is a minimal example of a Django site created using django-admin startproject

Click on the button below to deploy this repository with CI/CD on Elestio:

<a href="https://dash.elest.io/deploy?source=cicd&social=Github&url=https://github.com/elestio-examples/django"><img src="myapp\images\deploy-on-elestio.png" alt="Deploy on Elest.io" width="180px" /></a>

<img src="myapp\images\django.png" alt="screenshot of the Django app" width="100%" />

# Steps to clone this repository and run locally


### Step 1: Clone this repository

```
git clone YOUR_REPOSITORY_URL
```

### Step 2: Go to project folder.

```
cd django
```

### Step 3: Create a Virtual Environment.

```
pip install virtualenv
```

### Step 4: Activate the virtual environment.

```
virtualenv env
```

### Step 5: Install requirements.txt file.

```
pip install -r requirements.txt
```

### Step 6: Run your app in dev mode.

```
python manage.py runserver
```

### Step 7: Make some changes and push
Try to make some change in your Django project then push to the git repository

After few seconds to few minutes your change will be deployed on your CI/CD target 🚀
