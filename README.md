# OOAD-WEEK11
State Diagram

![](http://www.plantuml.com/plantuml/img/ROyn2W9134Nxd28N4FijP54FO6Svx68M1zP49d_kRyOTBSGgy7Xv9ADZAgYFbGWPg_1rWXG-Pt-AkXIYwh8xR3XzCG-SsmIVB6jp-9_KdQCXqX_hKiGzuIvfhe1fjDw80t57fdjR5leDndQB3FtAUUiIZQAt-E45)
```
@startuml

title Water Dispenser

use-> Water_Dispenser : insert Coin
use -> Water_Dispenser :insert Bottle
use -> Press_the_button : Press the button on/off
Water_Dispenser -> use : Water bottle


@enduml
```
