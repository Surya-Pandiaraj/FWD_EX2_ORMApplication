### NAME: SURYA P <br>
### REG NO: 212224230280 <br> 
### Date: 28/08/2025

## EX. No. 2 : ORM APPLICATION

## AIM :
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM :
<img width="799" height="678" alt="image" src="https://github.com/user-attachments/assets/a697cc03-d185-4c1a-b5e1-8e93b7aea489" />

## DESIGN STEPS :

### STEP 1
Clone the problem from GitHub

### STEP 2
Create a new app in Django project

### STEP 3
Enter the code for admin.py and models.py

### STEP 4
Execute Django admin and create details for 10 books

## PROGRAM :

## admin.py
```
from django.contrib import admin
from .models import Movies, MoviesAdmin
admin.site.register(Movies,MoviesAdmin)
from django.db import models
```

## Models.py
```
from django.contrib import admin
class Movies(models.Model):
    M_ID = models.IntegerField(primary_key=True)
    M_name = models.CharField(max_length=100)
    Release_date=models.DateField()
    Director=models. CharField(max_length=50)
    Actors=models. CharField(max_length=100)
 
class MoviesAdmin(admin.ModelAdmin):
    list_display=('M_ID', 'M_name', 'Release_date', 'Director','Actors')
```

## OUTPUT :

<img width="1917" height="613" alt="image" src="https://github.com/user-attachments/assets/e823c7b7-4787-47d8-bac7-b4d0f4b0a7df" />

## RESULT :
Thus the program for creating a database using ORM hass been executed successfully
