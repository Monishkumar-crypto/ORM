# Ex02 Django ORM Web Application
# Date:
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
```
admin.py

from django.contrib import admin
from .models import bankloan,userAdmin
admin.site.register(bankloan,userAdmin)

models.py

from django.db import models
from django.contrib import admin
class bankloan(models.Model):
    customer_name=models.CharField(max_length=100,primary_key=True)
    customer_id=models.CharField(max_length=100)
    loan_no=models.IntegerField()
    loan_amount=models.IntegerField()
    email=models.EmailField()
 
class userAdmin(admin.ModelAdmin):
    list_display=('customer_name','customer_id','loan_no','loan_amount','email')
```
# OUTPUT

![1](https://github.com/user-attachments/assets/75c9b45f-7172-41bb-b4ed-69c92d3744de)

![2](https://github.com/user-attachments/assets/9d5a3cea-eeb2-47f9-a28e-a59030fb0f40)

![3](https://github.com/user-attachments/assets/373e3c15-2e01-4737-979a-910b9b473292)
# RESULT

Thus the program for creating a database using ORM hass been executed successfully
