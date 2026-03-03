---
layout: default_dl
parent: Final Project
grand_parent: Advanced Topics
title: CW Solutions
nav_exclude: true
---

# cw-class-diagrams


```mermaid
classDiagram
    class House {
        +String address
        +Room main_room
    }
    class Room {
        +int square_feet
    }
    class Kitchen {
        +bool has_gas_stove
    }

    House *-- Room : contains
    Room <|-- Kitchen : inheritance
```

```
classDiagram
    class House {
        +String address
        +Room main_room
    }
    class Room {
        +int square_feet
    }
    class Kitchen {
        +bool has_gas_stove
    }

    House *-- Room : contains
    Room <|-- Kitchen : inheritance
```