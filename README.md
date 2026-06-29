# NGT's Data Jigsaw

## The vision

A scalable jigsaw puzzle app capable of providing 1,000, 5,000, or even 10,000+ piece puzzle builds. A user interface that can handle large piece counts elegantly with rapid piece sorting and placement tools. Some algorithmic "cheat" methods included for those who love the challenge without the tedium.

## The Problem 

Most commercial jigsaw puzzle apps set hard limits of less than 1,000 pieces. There may be many reasons for such limitations, but the biggest two problems come down to data structure and user interface. Individual critiques of desktop apps will be added below as I compare/contrast marketed offerings.

- [x] [Microsoft Jigsaw](/documentation/MSJigsaw.md)
 
## The Solution

By separating data structure from user interface all piece processing can happen at the data layer with precision and speed. The user interface can be reduced to lightweight draws of only visible pieces.  Theoretical unlimited desk space and intuitive tools allow the user to handle large piece counts elegantly.

### What This Is

- A data engineering approach
- A jigsaw hobbyist's dream
- A sample of my methodology for software development
- An open source project for desktop computers
- Just for the fun and entertainment value

### What This Is Not

- A casual game
- A mobile app
- A commercial product

## The Process

- Data structuring
- Data Proof of Concept
- Visual layout
- Individual component Proof of Concepts
- Putting it all together

### Data Structuring

When I start visualizing a new project I always like to break it down into some form of data structure. It might be a single spreadsheet or table; a relational database; or an object model. Data may take the form of numerical, strings, graphical, or even bitwise when that seems valid.

Knowing I wanted to scale piece counts in large numbers I initially thought of using Pandas dataframes for its rapid math and representing the data mostly numerically. Therefor, my initial ideas focused on the relationship between the pieces and the screen, but a relational database did not fit too well. I determined that the pieces themselves are fundamentally objects of the real world and should naturally follow object-oriented programming (OOP) principles.

Still, there are some relationships that must be observed, so I will refine the data structure by categories detailed in separate docs:

- [x] [Pieces](/documentation/Pieces.md)
  - [x] [Standard Shape Orientation](/documentation/Shapes.md)
- [ ] ⏳ [Connections](/documentation/Connections.md)
- [x] [Containers](/documentation/Containers.md)
- [ ] [Desktop Canvas](/documentation/Canvas.md)
- [ ] [Game Mechanics](/documentation/Mechanics.md)

## Disclaimers

As a fun project for my own entertainment progress on this project may come in small spurts of activity. Rome wasn't built in a day by hobbyists, and this project won't be either.

Nothing is set in stone. As a work in progress this README and any or all other files may be revised at any time.