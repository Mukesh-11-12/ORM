# Ex02 Django ORM Web Application
## Date: 10.05.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![434742095-9a3b8dfa-fa7d-4926-a797-9a9ea40322f5](https://github.com/user-attachments/assets/8db21f58-fd77-4fa4-8cab-68ce18b9a38d)



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

from .models import Movies,MoviesAdmin

admin.site.register(Movies,MoviesAdmin)
 
models.py

from django.db import models
from django.contrib import admin

class Movies(models.Model):
    Userid  = models.IntegerField(primary_key=True)
    Username = models.CharField(max_length=30)
    Email_Id = models.CharField(max_length=30)
    Phone_number = models.IntegerField()
    Moviename =  models.CharField(max_length=20)
    Show_date = models.DateField()
    Show_time = models.TimeField()
    No_of_seats = models.IntegerField()


class MoviesAdmin(admin.ModelAdmin):
    list_display = ('Userid','Username','Email_Id','Phone_number','Moviename','Show_date','Show_time','No_of_seats')

```
## OUTPUT
![Screenshot 2025-05-10 103726](https://github.com/user-attachments/assets/5ffe691d-3965-4f03-b90d-9dd62542f094)

Include the screenshot of your admin page.


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
