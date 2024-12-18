# Ex02 Django ORM Web Application
## Date: 28.10.24

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![Screenshot 2024-11-04 162422](https://github.com/user-attachments/assets/ae67dc99-9825-4204-b9a4-607470981aba)

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
```
admin.py

from django.contrib import admin
from .models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)

models.py

from django.db import models
from django.contrib import admin
class Loan (models.Model):
   name=models.CharField(max_length=100)
   loantype=models.CharField(max_length=100)
   age=models.IntegerField(max_length=3)
   aadharnumber=models.IntegerField(max_length=12)
   mobilenum=models.CharField(max_length=10)

class LoanAdmin(admin.ModelAdmin):
  list_display=('name','loantype','age','aadharnumber','mobilenum')
```
## OUTPUT

![Screenshot 2024-10-28 205114](https://github.com/user-attachments/assets/5573a90b-8781-4225-b9f5-4fa9163f8e3e)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
