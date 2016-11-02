# OOAD-WEEK11
State Diagram

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuUAArefLqDMrKyWlICqBoKXDoSylua9YW-MIS_ABKs6I2bnS3gbvAK3D0000)
```
@startuml

[*] --> openThedoor
openThedoor --> closeThedoor
 

@enduml
```

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuUBYYjQALT3LjLF8prEmoim3IkJaS07POA6qD2uWXafpSJcavgK0DG40)
```
@startuml

[*] --> on :install
on --> off
off --> on

@enduml
```

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuTBGqbJGrRLJKFB9Jy_CK-82iuCpq_FyIqiWFA0ABeVKl1IWQW00)
```
@startuml
(*) --> "Login"
--> "SignOut"
--> (*)
@enduml
```
