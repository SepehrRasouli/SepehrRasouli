```python
class Identity:
    def __init__(self,name:str,age:int,location:str):
        self.name = name
        self.age = age
        self.location = location

class Programmer:
    def __init__(self,specialty:str,familiar_with:list,interested_in:list):
        self.specialty = specialty
        self.familiar_with = familiar_with
        self.interested_in = interested_in
    
class Contact:
    def __init__(self,telegram:str,github:str,blog:str):
        self.telegram = telegram
        self.github = github
        self.blog = blog

identity = Identity(
    "Sepehr", 
    15, 
    "Tehran",
)

programmer = Programmer(
    "Back-End, Python Developer",
    ["Git","Javascript","Docker","Django","Linux"],
    ["Open-Source Community","Linux","Security","Machine Learning"],
)

contact = Contact(
    "t.me/SepehrRS",
    "You're Here !",
    "sepehrrs.blog.ir",
)
```
