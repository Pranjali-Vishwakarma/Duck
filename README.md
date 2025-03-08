# Ducks

## Overview
This Java program demonstrates the Strategy Design Pattern using different types of ducks. Each duck has different behaviors for flying, quacking, and swimming, which are implemented using separate interfaces and concrete classes.

## Features
- **Encapsulation of Behaviors**: Each behavior (quacking, swimming, flying) is encapsulated in separate classes, allowing flexibility in assigning behaviors dynamically.
- **Extensibility**: New duck types or behaviors can be added without modifying existing code, following the Open/Closed Principle.
- **Strategy Pattern Implementation**: Enables ducks to change their behaviors at runtime.

## Classes and Interfaces

### **Abstract Class:**
- `Duck`: The base class for all duck types. It contains references to `QuackBehaviour`, `SwimBehaviour`, and `FlyBehaviour` interfaces.

### **Interfaces:**
- `QuackBehaviour`: Defines the quacking behavior.
- `SwimBehaviour`: Defines the swimming behavior.
- `FlyBehaviour`: Defines the flying behavior.

### **Concrete Duck Classes:**
- `MallardDuck`: Implements specific behaviors for a Mallard Duck.
- `RedheadDuck`: Implements specific behaviors for a Redhead Duck.
- `RubberDuck`: Implements specific behaviors for a Rubber Duck.

### **Concrete Behavior Classes:**
- **Quack Behaviors:**
  - `Quack`: Implements normal quacking.
  - `Squeak`: Implements squeaking for RubberDuck.
- **Swim Behaviors:**
  - `SwimWithLegs`: Implements normal swimming.
  - `Floating`: Implements floating for RubberDuck.
- **Fly Behaviors:**
  - `FlyWithWings`: Implements normal flying.
  - `FlyNoWay`: Implements inability to fly.

### **Main Class:**
- `Main`: Demonstrates the functionality of different ducks by creating instances and invoking their behaviors.

## Usage
1. Compile the Java files:
   ```sh
   javac *.java
   ```
2. Run the program:
   ```sh
   java Main
   ```
3. The output will display different ducks performing their respective behaviors.

## Example Output
```
-------------
I am a mallard duck.
Quackkkkk!
I believe I can swim
I can fly!
-------------
I am a rubber duck
Squeakkkkk!
I am afloat
I can't fly :(
-------------
I am a redhead Duck
Quackkkkk!
I believe I can swim
I can fly!
------------
```

## Future Enhancements
- Implement new duck types.
- Add more behaviors dynamically.
- Introduce a graphical user interface (GUI) for better visualization.

## Author
Pranjali Vishwakarma

