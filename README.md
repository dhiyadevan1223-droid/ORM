# Ex01 Django ORM Web Application
## Date: 25-11-25

## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM
```
models.py
from django.db import models
from django.contrib import admin

# Create your models here.
class cars(models.Model):
    car_name=models.CharField(max_length=50)
    car_model=models.CharField(max_length=50)
    car_id=models.IntegerField()
    car_colour=models.CharField(max_length=50)


class carsAdmin(admin.ModelAdmin):
    list_display=['car_name','car_model','car_id','car_colour']


admin.py
from django.contrib import admin
from.models import cars,carsAdmin

admin.site.register(cars,carsAdmin)
```

## OUTPUT

<img width="1871" height="930" alt="image" src="https://github.com/user-attachments/assets/7456f3bf-2994-4677-9041-83493ea3f1bc" />


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
