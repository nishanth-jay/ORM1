# Ex01Django ORM Web Application
# Date: 26.11.2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 cars

# PROGRAM
```
models.py:
from django.db import models
from django.contrib import admin

class Car(models.Model):
    plate_no = models.IntegerField()
    car_model = models.CharField(max_length=100)
    car_type= models.CharField(max_length=100)
    engine_type = models.CharField(max_length=100)
    color = models.CharField(max_length=100,default="")

class CarAdmin(admin.ModelAdmin):
    list_display = ['car_model', 'car_type', 'engine_type','color']
```
```
admin.py:
from django.contrib import admin
from .models import Car,CarAdmin


admin.site.register(Car,CarAdmin)
```
# OUTPUT
<img width="1910" height="1021" alt="Screenshot 2025-11-26 092219" src="https://github.com/user-attachments/assets/b2803e14-f06f-4478-88d8-781ee406d385" />


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
