```python
def WhoAmI(**kwargs):
    print("Who Am I ?")
    print(f"Hi ! My name is {kwargs['name']}")
    print(f"I'm {kwargs['age']} Years Old & I Live in {kwargs['city']}")
    print(f"I'm a Beginner {kwargs['developer']} developer, And I'm always eager to learn new things !")
    print(f"I'm Currently Learning {kwargs['learning']}")
    print(f"My Favorties Are => {kwargs['favorites']}\n")


def ShowStatus(**kwargs):
    print("My Status : ")
    print(f"I'm Currently * {kwargs['employed']} *")
    print("My Skills & Their status Are :")
    for skill, status in zip(kwargs['skills'].keys(), kwargs['skills'].values()):
        print(f"{skill} ****  {status}" + "\n"*(skill == list(kwargs['skills'].keys())[-1]))
    
    


def ShowContactInfo(**kwargs):
    print("My Contact Info :")
    print(f"My Github Page is => {kwargs['github']}")
    print(f"My Blog Is => {kwargs['blog']}")
    print(f"My Email Address Is => {kwargs['email']}\n")


WhoAmI(
    name="Sepehr Rasouli",
    age=15,
    city="Tehran",
    developer="Back-End Developer",
    learning="Django , Linux And Many Other Things !",
    favorites="Python - Django - Linux - Open-Source Projects - English - Lo-Fi Music :D"
)

ShowStatus(
    employed="Not Employed",
    skills={"Python": "Good | Learning",
            "Django": "Just Learning !",
            "English": "Good | Learning",
            "Linux": "Eh... | Learning",
            "Other languages": "Learning !!"
            }
)

ShowContactInfo(
    github="https://www.github.com/SepehrRasouli",
    blog="sepehrrs.blog.ir",
    email="sepehrrs06@gmail.com",
)

```
