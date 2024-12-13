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
Include the screenshot of your admin page.
![Screenshot 2024-12-07 045318](https://github.com/user-attachments/assets/6ee32a5c-0a2d-4175-a379-51af18ccb55d)

![Screenshot 2024-12-07 045613](https://github.com/user-attachments/assets/a52bda47-d65d-4f39-8fda-01087230299a)
![Screenshot 2024-12-07 045634](https://github.com/user-attachments/assets/c7163a8b-a9bd-4e19-b300-0f0e6f78e39c)
![Screenshot 2024-12-07 045648](https://github.com/user-attachments/assets/34b13ba3-a13e-404b-a7a1-387c09438663)
![img](https://github.com/user-attachments/assets/fcb01a7e-c24a-4783-947f-3fc4d2c6b3a2)





# RESULT
Thus the program for creating a database using ORM hass been executed successfully
