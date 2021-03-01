[![Build Status](https://travis-ci.com/cl598/219isoopdesign.svg?branch=master)](https://travis-ci.com/cl598/219isoopdesign)

Structural Pattern : **Adapter**

    Allows objects with incompatible interfaces to collaborate

Here, you can see the old interface with **operation** methods for addition
and subtraction.

![structure_1](/img/sa1.png)

Next, you see the new interface with **separate** methods used for addition
and subtraction.

![structure_2](/img/sa2.png)

We create an adapter class for the calculator that **wraps** around the 
new interface to add the **operation** methods for the public view.

The **separate** methods are used, but in a private view.

![structure_3](/img/sa3.png)

Creational Pattern : **Singleton**

    Class having only one instance while having a global 
    access point to this instance

Constructors, as a default, are set to be private to avoid other objects from
using the operators with the _singleton_ class.

![creational](/img/singleton.png)

Behavioral Pattern : **Chain of Responsibility**

    Allows an access to pass requests along a chain
    of handlers
    
    As one receives a request, each handler decides
    whether to process the request or pass the request
    to the next handler in the chain

Chain of responsibility is processed/passed through **handlers**, which are methods.
Each handler stores its own reference to the next handler through the chain,
and the requests continue to pass through all handlers until each had a chance
to process the request.

![behavioral](/img/chain.png)

### Codes and References
https://betterprogramming.pub/javascript-design-patterns-25f0faaaa15

https://refactoring.guru/design-patterns/chain-of-responsibility
