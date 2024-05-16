# Ex 02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![f1](https://github.com/Surekaelango/ORM/assets/127727904/ade8b988-32fa-482c-b725-ea4be36b15c0)

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
model.py
```

from django.db import models
from django.contrib import admin
class Library_DB(models.Model):
    serial=models.IntegerField(primary_key=True);
    title=models.CharField(max_length=20);
    author=models.CharField(max_length=20);
    publishion=models.CharField(max_length=20);
    price=models.IntegerField();
class Library_DBAdmin(admin.ModelAdmin):
    list_display=("serial","title","author","price");
```
admin.py
```
from django.contrib import admin
from .models import Library_DB,Library_DBAdmin
admin.site.register(Library_DB,Library_DBAdmin)
```


## OUTPUT
![f2](https://github.com/Surekaelango/ORM/assets/127727904/3ae8e081-124d-49b5-9e2d-e3063067a8f8)





## RESULT
Thus the program for creating a database using ORM hass been executed successfully
