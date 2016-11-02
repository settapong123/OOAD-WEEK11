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

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuUAArefLqDMrKmXAJKofv0AJOBvhHMfoQKbcNZeNd8Ma3bNCgJGjBRK8f1RE0eldbvOKb9PmGIY4PYw7rBmKeEK0)
```
@startuml

[*] --> Ready
Ready --> Executing
Executing --> Ready
Executing --> Buffering
Buffering --> output
output--> Ready

@enduml
```
# Activity Diagram

![](http://www.plantuml.com/plantuml/img/JKyn3i8m3DppYbCcG0fFG1rWHGX6w10bhXefJQl4HUhlSQ5KzUBJ-Su-LuLjvh6BYWD7mfbYU5EUe7Q7FOmvGT_wmfrDMYq0nWljLw4A3JGmB5FNTxHENyacZqmk384I7wKqkAMay5tpbFCJBACLLmtz896NqJagHVyrb-Hhp77a5iL2Cv-5l_QyiTwfY7as_H3Ck8cfX0cDggJ9iny0)
```
@startuml
title Delivery 
(*) --> "Postman"
Postman -d-> delivery 

if "  postman come delivery\nand recipient...." then
  -d->[stay at home] "Send success"
  -d->[End] (*)  

else
  -r->[Not at home] "Resend"
  Resend -u-> delivery
endif
@enduml
```

![](http://www.plantuml.com/plantuml/img/DS_12eCm30RWUvuYzBGDV0NnC8N1ODwTXwAfbdMnj96z_g9pfuO_V7zebSKcMTy1n4iWR1FbZ38Jve-NOKRB8mO_pGAdoncBeaHpuxWABf6I5R-m0V1EKxUpk1VyiDaI1jnO9scb7iszlc8MFxoCvhf9sjZLF7gUyCanBOFwNcy1XKoRBJjdTJpiesdCqNYely4TQUO0AdtrKry0)
```
@startuml
title Press the switch and light
(*) --> "Input operation"

if "If the press switch" then
  -->[true] "LED stick"
    -r-> [Ending \nprocess](*)
else
  ->[false] "LED OFF"
  -->[Ending process] (*)
endif

@enduml
```

![](http://www.plantuml.com/plantuml/img/JO-n2eCm54NtVCKbKrkG3bsB2DAvq5KSeddMOF8YCMdnxnlhulI6Uyxblcg9AiJah8WcMiABOWgCplj9d2vd54K9wSXr5AGm0sGzKZyPVcEcOBpEP0Z-InfttA3LAX57Oe7DR7QnXJpKofoHNMX3okRveQ0JNMUrmdccDSEridsoAXhF60oJtDkEq_xkWtMBF58GQpE8Af_yo0y0)
```
@startuml
title Return book
(*) --> "member"
if "Checking period borrowed < 3 day" then
  -->[member] "Return book"
  else
  ->[Overdue/pay money] "Calculation fine"
  -->Return book
  ->[End] (*)
endif
@enduml
```
