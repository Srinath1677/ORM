# Ex01 Django ORM Web Application
## Date: 

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
class car(models.Model):
    car_name=models.CharField(max_length=20)
    year=models.IntegerField()
    color=models.CharField(max_length=10)
    registration_no=models.IntegerField(primary_key=True)
    model=models.CharField(max_length=20)
class carAdmin(admin.ModelAdmin):
    list_display=["car_name","year","color","registration_no","model"]


admin.py
from django.contrib import admin
from .models import car,carAdmin
admin.site.register (car,carAdmin)
```


## OUTPUT

<img width="1920" height="1080" alt="Screenshot 2025-09-20 012607" src="https://github.com/user-attachments/assets/7055c349-473d-437d-bde3-28802d833e1a" />


## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
