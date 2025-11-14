<img width="940" height="506" alt="505150514-6a96f356-bc03-4c5a-a155-c9e960ec7933" src="https://github.com/user-attachments/assets/02860bb9-30ce-442f-9744-e00687e64e9c" /># Ex02 Django ORM Web Application
## 

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

<img width="940" height="506" alt="505150514-6a96f356-bc03-4c5a-a155-c9e960ec7933" src="https://github.com/user-attachments/assets/bae2fd90-43b4-4e53-a97f-87197470810e" />

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
## Admin.py
```py
from django.contrib import admin
from . models import Car


admin.site.register(Car)

class CarAdmin(admin.ModelAdmin):
    list_display = ('id','brand','model','year','price')
```

## Models.py
```py
from django.db import models

class Car(models.Model):
    id = models.IntegerField(primary_key=True)
    brand = models.CharField(max_length=15)
    model = models.CharField(max_length=30)
    year = models.DateField()
    price = models.IntegerField()
```




## OUTPUT

<img width="1917" height="1080" alt="Screenshot 2025-11-10 221647" src="https://github.com/user-attachments/assets/e321013b-17a5-4c65-9ba2-e7db64280cae" />



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
