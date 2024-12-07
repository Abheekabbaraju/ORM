# Ex02 Django ORM Web Application
# Date:1/12/24
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
~~~
from django.db import models
from django.contrib import admin

class Book(models.Model):
    Book_name = models.CharField(max_length=20)
    Book_id= models.CharField(max_length=100)
    Mobile_no = models.IntegerField()
    Age = models.IntegerField()
    Email = models.EmailField()
    DoB = models.DateField()
    Book_amount = models.IntegerField()

class BookAdmin(admin.ModelAdmin):
    list_display = ('Book_name', 'Book_id', 'Mobile_no', 'Age', 'Email', 'DoB', 'Book_amount')
~~~
##admin:
~~~
from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book, BookAdmin)
~~~
# OUTPUT
Include the screenshot of your admin page.
![Screenshot (50)](https://github.com/user-attachments/assets/d8dabf49-27fc-47f1-825a-42e6a1c0972a)
![Screenshot (51)](https://github.com/user-attachments/assets/bd6133c9-1275-44e9-842c-03baf92ce4d4)
![Screenshot (52)](https://github.com/user-attachments/assets/0567396b-529c-4d91-9986-ef083bf2795f)
# RESULT
Thus the program for creating a database using ORM hass been executed successfully
