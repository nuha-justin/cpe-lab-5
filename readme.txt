= Lab 5: Composition

== Overview
The purpose of this lab is to improve understanding of classes and composition.

== Instructions

. Refactor the `main.cpp` class
.. The `main.cpp` file includes the definition of the `Person` class. Create the files `person.cpp` and `person.h` and move the `Person` code in `main` to the cpp and h files. The h file should contain the class definition. The cpp file should contain the implementation of the class.
.. Modify the `makefile` as needed so that the program compiles and check that the program functions correctly.

. Create the `Heart` class
.. Create a class called `Heart` that has one integer attribute called `rate`
.. Add getters and setters for `rate` attribute
.. Add a parameterized constructor that takes the `rate` value as its argument
.. Add a method `ok()` that that returns
true if the value of `rate` is greater than 50
.. Modify the `makefile` as needed to add the new class (cpp and h) to the project

. Add the `Heart` class to the `Person` class
.. Modify the `Person` class to have an attribute `Heart heart`. *Do NOT add getters and setters for the heart attribute. The class should not be externally accessable.*
.. Modify the `Person` constructor to include the heart rate. This rate should be used to
initialize the `Heart` attribute.
.. Add a method called `heartOK` to the `Person` class that returns true or false based on whether the heart `ok` method returns true or false

. In the `main` method, add a call to the `Person` `heartOK` method and print out the results to the console.