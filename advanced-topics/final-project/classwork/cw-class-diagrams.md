---
layout: default_dl
parent: Final Project
grand_parent: Advanced Topics
title: CW Class Diagrams
nav_order: 110
---

# Classwork(CW): Class Diagrams

## Mapping the House

**Objective:** Translate Java source code into a visual UML Class Diagram using Mermaid syntax.

## Source Code

Analyze the following Java classes. Look closely at how the classes relate to one another. Pay attention to **inheritance** (subclassing) and **composition** (one class containing another).

```java
// The Base Class
public class Room {
    public int squareFeet;
    private String wallpaperColor; 
}

// The Subclass
public class Kitchen extends Room {
    public boolean hasDishwasher;
}

// The Container Class
public class House {
    public String address;
    public Room masterBedroom; 
}

```

## Instructions

1. Navigate to [Mermaid.live](https://mermaid.live/).
2. In the left-hand code editor, use the `classDiagram` syntax to recreate these three classes.
3. **Requirements for your diagram:**
* Show **public** variables using the `+` symbol.
* Show the **private** variable using the `-` symbol.
* Represent the **Inheritance** relationship (Kitchen *is a* Room) using `<|--`.
* Represent the **Composition** relationship (House *has a* Room) using `*--`.


## Syntax Reminders

| Relationship | Mermaid Syntax | Description |
| --- | --- | --- |
| **Inheritance** | `Parent < | -- Child` |
| **Composition** | `Container *-- Contained` | "Has a" (ownership) relationship |
| **Public** | `+` | Visible to all |
| **Private** | `-` | Hidden/Internal |

---

## Check-off Criteria

To get credit for this activity, please raise your green popsicle once your diagram on Mermaid.live matches the following:

* [ ] All 3 classes (`House`, `Room`, `Kitchen`) are present.
* [ ] `Kitchen` points to `Room` with an inheritance arrow.
* [ ] `House` connects to `Room` with a composition diamond.
* [ ] `wallpaperColor` is correctly marked as private.
