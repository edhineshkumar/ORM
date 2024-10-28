## Date: 28.10.2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
![Screenshot 2024-10-28 205114](https://github.com/user-attachments/assets/26f402f5-08e8-434d-96ea-8dc7aaccc9e7)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
