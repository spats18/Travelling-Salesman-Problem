# Travelling-Salesman-Problem
## SOLID principles and Wirth and Parnas:
We have carefully incorporated the SOLID principles to ensure clean coding. While Implementing the concepts of Object-oriented programming, we have made sure to keep our code readable and well-documented. We have specified the access as private for the information that is not required for the user to know.
#### Single Responsibility Principle:
We have divided the responsibility among all the classes. For instance, the Graphics class will manage the GUI for our assignment and doesn’t have any other functionality like computing the result. Furthermore, we have designed different classes to handle Asymmetric and Symmetric data. Also, Our algorithm to figure out the minimum path lies in a separate Class.
#### Open-Closed Principle:
The Data class earlier was supposed to handle the files and parse the data. The goal was to return the ArrayList of coordinates. The limitation was, our algorithm required the 2-D matrix to work upon. Later, we implemented AsymmetricData and SymmetricData classes instead of modifying the code in the Data class. So we made sure that our classes are open for extension but not for modification. 
#### Liskov Substitution Principle:
The Data class returned the ArrayList of coordinates. The limitation was, our algorithm required the 2-D matrix. AsymmetricData and SymmetricData classes inherit the Data class. Both these classes are better than their parent in terms of returning the more refined data parsing for the algorithm to compute the result.
#### Interface Segregation Principle:
We have programmed different interfaces depending on the requirement, instead of a general-purpose Interface. Every class is clear about which interface to implement and what functions to include as a part of the requirement.
#### Dependency Inversion Principle:
We have implemented interfaces for all the classes. We are using the references of interfaces to call the object of classes that implements the given interface. For instance, the reference of ShortestPathInterface is calling all the methods of the class GetShortestPath. Similarly, for all the classes, we have inverted the dependency on interfaces.

## Class Diagram
![] (TSP_Class%20Diagram.png)
