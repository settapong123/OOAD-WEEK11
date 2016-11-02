# OOAD-WEEK11
State Diagram

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuUAArefLqDMrKyWlICqBoKXDoSylua9YWwIIS_ABKs5oo1oG950_5vT3QbuAq3G0)
```
@startuml

[*] --> openThedoor
openThedoor--> closeThedoor
closeThedoor--> [*]

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

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuTBGqbJGrRLJo4zBumBJUI3AAJ-_14G7fIQcL8B5WUgu75BpKe1w0000)
```
@startuml
(*) --> off
--> on
-->Boot
-->Ready
--> (*)
@enduml
```
