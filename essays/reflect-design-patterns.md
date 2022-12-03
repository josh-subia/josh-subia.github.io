---
layout: essay
type: essay
title: "Design Patterns in Practice"
# All dates must be YYYY-MM-DD format!
date: 2022-12-01
published: true
labels:
  - Software Engineering
  - Web Development
  - Design Patterns
---
UI frameworks make web development so much easier.
## My Life Could Have Been So Much Easier
<div>
<img src = ../img/reflect-design-patterns/trash-computer.gif width="200px" align="left" style="margin-right: 1em">
Despite my 4+ years of experience dealing with college assignments and problems, it never ceases to amaze me how many times I spent way much time trying to solve a problem that could have been solved rather quickly or even avoided completely. After about an hour or so trying to solve such a simple problem, I feel like doing something like the gif on the left. All of these troubles and pains could have been avoided if I had utilized a design pattern, which are typical solutions to common problems. Design patterns helps prevent subtle issues early in the development stage so that they do not become a much larger problem later. Patterns are often confused with algorithms, which gives precise steps to achieve an objective, while patterns are more like a blueprint, where you can only see the end result and what some of its components are, but are without steps, as its implementation is up to you to decide. 
</div>

## Different Design Patterns
The concept of patterns was first described by Christopher Alexander in his book "A Pattern Language: Towns, Buildings, Construction.", describing patterns as a "language" for designing an urban environment. This concept was picked up by Erich Gamma, John Vlissides, Ralph Johnson, and Richard Helm, who then published a book in 1994 called "Design Patterns: Elements of Reusable Object-Oriented Software", where the concept of patterns was applied to software engineering. Currently, design patterns are classified into three main types: Creational, Structural, and Behavioral. 

Creational design patterns are design patterns that deal with object instantiation, specifically trying to create objects that are suitable for the current system. Creational design patterns control object creation by utilizing the following components: Abstract Factory, Builder, Factory Method, Object Pool, Prototype, and Singleton. 

Structural design patterns ease the design of systems by identifying a simple way to instantiate relationships between entities, and utilizes the following components: Adapter, Bridge, Composite, Decorator, Facade, Flyweight, Private Class Data, and a Proxy.

The last main type of design pattern is the behavioral design pattern. Behavioral design patterns identify communication patterns between objects to increase flexibility in their communications. The table below shows all of the components and their function for the three design types. 

<table>
    <tr>
        <th>Creational Design Patterns</th>
        <th>Description</th>
    </tr>
    <tr>
        <td>Abstract Factory</td>
        <td>Creates an instance of several families of classes</td>
    </tr>
    <tr>
        <td>Builder</td>
        <td>Separates object construction from its representation</td>
    </tr>
    <tr>
        <td>Factory Method</td>
        <td>Creates an instance of several derived classes</td>
    </tr>
    <tr>
        <td>Object Pool</td>
        <td>Avoid expensive acquisition and release of resources by recycling objects that are no longer in use</td>
    </tr>
    <tr>
        <td>Prototype</td>
        <td>A fully intialized instance to be copied or clones</td>
    </tr>
    <tr>
        <td>Singleton</td>
        <td>A class of which only a single instance can exist</td>
    </tr>
    <tr>
        <th>Structural Design Patterns</th>
    </tr>
    <tr>
        <td>Adapter</td>
        <td>Math interfaces of different classes</td>
    </tr>
    <tr>
        <td>Bridge</td>
        <td>Separates an object's interface from its implementation</td>
    </tr>
    <tr>
        <td>Composite</td>
        <td>A tree structure of simple and composite objects</td>
    </tr>
    <tr>
        <td>Decorator</td>
        <td>Add responsibilities to objects dynamically</td>
    </tr>
    <tr>
        <td>Facade</td>
        <td>A single class that represents an entire subsystem</td>
    </tr>
    <tr>
        <td>Flyweight</td>
        <td>A fine-grained instance used for efficient sharing</td>
    </tr>
    <tr>
        <td>Private Class Data</td>
        <td>Restricts accessor/mutator acces</td>
    </tr>
    <tr>
        <td>Proxy</td>
        <td>An object representing another object</td>
    </tr>
    <tr>
        <th>Behavioral Design Patterns</th>
    </tr>
    <tr>
        <td>Chain of Responsibility</td>
        <td>A way of passing a request between a chain of objects</td>
    </tr>
    <tr>
        <td>Command</td>
        <td>Encapsulate a command request as an object</td>
    </tr>
    <tr>
        <td>Interpreter</td>
        <td>A way to include language elements in a program</td>
    </tr>
    <tr>
        <td>Iterator</td>
        <td>Sequentially access the elements of a collection</td>
    </tr>
    <tr>
        <td>Mediator</td>
        <td>Defines simplified communcation between classes</td>
    </tr>    
    <tr>
        <td>Memento</td>
        <td>Capture and restore an object's internal state</td>
    </tr>    
    <tr>
        <td>Null Object</td>
        <td>Designed to act as a default value of an object</td>
    </tr>    
    <tr>
        <td>Observer</td>
        <td>A way of notifying change to a number of classes</td>
    </tr>    
    <tr>
        <td>State</td>
        <td>Alter an object's behavior when is state changes</td>
    </tr>    
    <tr>
        <td>Strategy</td>
        <td>Encapsulates an algorithm inside a class</td>
    </tr>    
    <tr>
        <td>Template Method</td>
        <td>Defer the exact steps of an algorithm to a subclass</td>
    </tr>    
    <tr>
        <td>Visitor</td>
        <td>Defines a new operation to a class without a change</td>
    </tr>
</table>

## Patterns in Practice
<img src= "../img/reflect-design-patterns/flappy-bird.png" align="right" style="margin-left: 1em;" width="250px"> 
I first started looking into the different types of design patterns, I thought I did not utilize any of them before. However, after reading more into what design patterns are, I realized that I have used design patterns, specifically creational design patterns. In my Computational Media Systems class, I remember trying to replicate the game 'Flappy Bird' while adding a few extra functionalities. Since the game was basically endless, I needed to find a way to create an infinite number of pipes, if needed. Instead, I was able to use the object pool method to recycle these pipes instead of creating and then destroying them by moving the pipes back to the front of the queue once they have gone behind the player. I also utilized the singleton instance in my game 'Flappy Bird 2.' There were other instances in that class where I had to create infinitely spawning enemies or instantiate bullets and utilized creational design patterns. Over the course of ICS 314, I was also introduced to several components of the Behavioral design patterns such as chain of responsibility, iterator, and observer. However, I have yet to utilize structural design patterns. 

## Using Patterns to Predict the Future
While I have not utilized many of the design patterns mentioned above, if patterns suggest anything, its that I will probably utilize it sometime in the future without knowing it. Who knows, maybe more design patters will emerge that will solve more problems within software engineering and allow us to create even more powerful and complex systems. 