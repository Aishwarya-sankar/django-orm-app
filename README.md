# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from github.
### STEP 2:
Create a new app.
### STEP 3:
Enter the code for admin.py and models.py
### STEP 4:
Create django app and add student details.
## PROGRAM
```
models.py 

from django.db import models
from django.contrib import admin


class Student(models.Model):
    referencenumber=models.CharField(primary_key=true,max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')

admin.py

from django.contrib import admin
from myapp.models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)
```

## OUTPUT
SERVER OUTPUT
![server output 1](https://user-images.githubusercontent.com/121418444/232555509-88b6da96-bfb2-4297-84e2-4804a1344519.jpg)

CLIENT OUTPUT
![2023-04-06 (1)](https://user-images.githubusercontent.com/121418444/232555039-03da4fe4-317a-4096-a1b2-3233e72e2cc5.jpg)


## RESULT
Program executed successfully.
