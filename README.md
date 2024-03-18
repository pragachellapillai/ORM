# Ex02 Django ORM Web Application
## Date: 11/03/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![WhatsApp ](https://github.com/pragachellapillai/ORM/assets/148254952/29112981-0a1e-4e68-bf65-5e179d1bd0e4)



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
Models.py
```
from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
  Booknum=models.IntegerField(primary_key="Booknum");
  title=models.CharField(max_length=15);
  Author=models.CharField(max_length=20);
  Date=models.DateField();
  lang=models.CharField(max_length=10);
  price=models.IntegerField();
class Book_DBAdmin(admin.ModelAdmin):
  list_display=("Booknum","title","Author","Date","lang","price");

```
Admin.py
```
from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)
```
Include your code here

## OUTPUT

![Screenshot 2024-03-11 140203](https://github.com/pragachellapillai/ORM/assets/148254952/2a97d90f-f39c-480d-97cd-edfa3ef6ca52)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
