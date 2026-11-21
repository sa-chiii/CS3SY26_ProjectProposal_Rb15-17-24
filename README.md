# CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template: 

### Project Title or Name of the Application	: The Tom's Up Pet Shop
### Section			   	      : 9-Rubidium
### Group Members			    : LOARES, Cleo, MAGHUYOP, Lia, REMIGIO, Luis
### Date (Proposal Date)  : November 21, 2026

### Project Description:

- The Tom's Up Pet Shop... [at least 4 sentences]

**How does it work?**
- In this program, we have 7 classes: 
    1. Pet - Parent class; blue print for all pets with shared survival stats. Its attributes include: name, species, hunger, happiness, and energy. Its methods include: name_pet(), feed(), sleep(), play(), make_sound(), and check_status()
    2. PetShop - Displays available pets and lets user adopt one. Its only attribute is available_pets (list), and its methods include: diespl_pets(), and adopt_pet()
- Then we have 5 child classes which will inherit from Pet as well as have a unique attribute and method:
  1. Dog - Attribute: loyalty; Methods: fetch() _--> boosts happiness and loyalty, uses energy_.
  2. Cat - Attribute: curiosity; Methods: chase_laser() _--> boosts happiness and curiosity, uses energy_.
  3. Fish - Attribute: water_cleanliness; Methods: clean_tank() _--> restores water_cleanliness to 100 and boosts happiness_
  4. Bird - Attribute: singing_skill; Methods: sing() _--> increases singing_skill and happiness_
  5. Bunny - Attribute: fluffiness; Methods: brush_fur() _--> increases fluffiness and happiness, uses a little energy_
  
- Each pet will also override the make_sound method from the parent and make their own sound.
- Attributes such as hunger, happiness, energy, and every special attribute for each class will be integers from 1-100.
- Every action (e.g. feed, play, sleep, or special action), the pet's stats update dynamically and passing time slightly increases hunger and lowers energy.

**Who are our target users?**
- The primary demographic of Tom's Up Pet Shop are Junior High School students (ages 12-16) as well as casual gamers who enjoy virtual pet games. This includes students who want a fun, cozy game for leisure and animal lovers!

**Sample class Diagram from https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png:**

![Sample Diagram](https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png)

The Tom's Up Pet Shop UML Diagram ( https://www.canva.com/design/DAHbiyjlq8s/vGiem0xQE0bymyHopwNK6g/edit?ui=e30 )

### Goals:
[insert long-term outcomes]

- Objective 1: To design and develop an object-oriented system with the basic principles of OOP using encapsulation, inheritance, and polymorphism.

- Objective 2: To build an interactive pet adoption and care simulation where users can adopt and name a pet from a virtual pet shop and manage its survival stats through daily care actions.

[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
