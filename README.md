# Ex02 Django ORM Web Application
# Date:20/10/24
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
## models.py
~~~
from django.db import models
from django.contrib import admin

class Book(models.Model):
    book_no = models.CharField(max_length=100)
    book_name= models.CharField(max_length=100)
    author_name=models.CharField(max_length=100)
    email=models.EmailField()
    buyer_name=models.CharField(max_length=100)
    mobile_no=models.CharField(max_length=100)
class BookAdmin(admin.ModelAdmin):
    list_display = ('book_no','book_name','author_name','email','buyer_name','mobile_no')

~~~
## admin.py
~~~
from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book,BookAdmin)

~~~
# OUTPUT
![image](https://github.com/user-attachments/assets/cccec30a-5e25-42b6-b833-e6cbb1963e16)
![image](https://github.com/user-attachments/assets/513e48e2-75b8-417b-943a-fa25431a1e94)
![image](https://github.com/user-attachments/assets/d3d32f51-c7b8-44a8-847f-5278dc400ece)
![image](https://github.com/user-attachments/assets/6d9e9107-c893-4bf8-ab14-42bc54fd2130)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
