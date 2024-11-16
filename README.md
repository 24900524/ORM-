# Ex02 Django ORM Web Application
## Date: 12.11.2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).


## ENTITY RELATIONSHIP DIAGRAM
![project_web 1](https://github.com/user-attachments/assets/5df7d00b-b59f-49b4-9b7f-a0bdde9b782b)


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
from .models import Customer,CustomerAdmin
admin.site.register(Customer,CustomerAdmin)
  

 models.py

 from django.db import models
from django.contrib import admin
class Customer (models.Model):
    eid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class CustomerAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

```




## OUTPUT:  

![Screenshot 2024-11-14 143500](https://github.com/user-attachments/assets/b0687fad-7b13-4b1a-82b1-a6f6a7e5cb44)





## RESULT
Thus the program for creating a database using ORM hass been executed successfully
