# WEEK 4 - SOFTWARE DESIGN TASK ANSWERS 👩🏽‍💻⭐️

--------------------------------------------------------------------------------------------------------------------

**1. What do we mean by coupling and cohesion when discussing structured design?**

Both terms describe relationships/interactions between different components or modules within a software system. 

Cohesion: *the degree to which elements within a module or component are related/function together as a unified whole.* 

Coupling: *the degree of interdependence between different modules or components within a software system.* 


i.e. intra-module (cohesion) vs. inter-module (coupling).

Cohesion is desirable - it helps in creating modular, maintainable, reuseable code. 
Coupling should be minimised - want loosely coupled systems. 




**2. What is the difference between top-down and bottom-up design? Which best describes a function oriented design?**

Top-down design: *testing process starts from the top module and moves downwards; focuses on designing and testing the top module BEFORE integrating it with sub-modules.* 

Bottom-up design: *testing process starts in lower levels first and then works up the hierarchy; sub-modules combined first, tested and then process moves upwards towards the top module.* 


Function Oriented Programming is a top-down methodology, as the process starts with a high-level description of what the software does, then specifies in great detail the functionality of each smaller part.




**3. In which design methodology would a class diagram be most useful?**

A class diagram (i.e a diagram used to design/model software by describing classes and their relationships) would be most useful in the Object Oriented Programming, as the design structure relies on objects interacting in various ways, that make up the software system. 




**4. What are the four pillars of object oriented programming? Give a single-sentence description of each.**

Abstraction: *Hides away the implementation details inside something else meaning you can provide a generic function or object to work in various/multiple places. i.e. when calling a method, can just type the method signature not the full method + inner workings itself, which can be hidden inside another class elsewhere and imported.*

Encapsulation: *Limiting access to parts of code by setting access modifiers to private and making them accessible to a single class only, thereby protecting them.*

Inheritance: *Allows an object to acquire the properties and methods of another object.*

Polymorphism: *Enables the sharing of behaviours between objects via loose-coupling.*




**5.What is the strategy pattern? How would its implementation differ between a functional and object oriented system?**


The Strategy Pattern is a behavioural design pattern that enables dynamic change to the behaviour of an object, via encapsulation into different strategies. An object can choose from multiple algorithms and behaviours at runtime, (in contrast to statically choosing a single one), thus making it more flexible and reusable as different strategies can be added or modified without changing the core code of the object. This is achieved by extracting the behaviour of an object out into a separate class, (i.e. away from the main object), then swapping it in or out at runntime depending on our preferences. 

This design pattern is very useful in Object Oriented Programming as it provides a flexible way of encapsulating behaviours of objects which can then be applied to various different objects as/when required.
It would be very difficult to implement this pattern in Functional Programming, as the hierarchical structure doesn't lend itself well to interchanging behaviours, in addition to each sub-module being designed with a very specific function in mind. 




**6.Imagine you are creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.**

I think Object Oriented Programming would be most appropriate in this case as it provides a great deal of flexibility through polymorphism and abstraction, meaning it is suitable for projects with changing user requirements, such as in this case, as the application must adapt to whichever business type the user requires. This design method also enables the code to be reusable and scalable, through encapsulation, which again would be useful in this example, as the client could be a small local boutique clothing store handling 50 payments a month, or they could be a nation-wide established garage handling 100 payments per day. 
