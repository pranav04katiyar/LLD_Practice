Pillar 1: ENCAPSULATION -
Wrapping up of data (state) and methods (behavior) together into a single unit (i.e. class) and also hiding the data from outside world (i.e. data hiding).

How Encapsulation implements OOPs concept?
1. Maintainability - Encapsulated code easy to maintain.
2. Flexibility - Encapsulated code is easy to change.
3. Testability - Encapsulated code is easy to test.
4. Modularity - Encapsulated code is easy to divide in relevant state and behavior based on functionality.

Encapsulation has two aspects:
1. A language construct that facilitates the bundling of data with the methods (or other functions) operating on that data: Class
2. A mechanism for restricting direct access to some of the object's components: Access Modifiers (private, protected, public, default(package protected))

Concepts within Encapsulation:
1. Class & Object
    1.1. Attributes (or Properties or Fields) - Variables
    1.2. Methods (or Behaviors) - Functions
    1.3. Constructor                           //Special type of method which is used to initialize the object
        1.3.1. Default Constructor                  //If we don't define any constructor, then compiler will provide default constructor, which is empty
        1.3.2. No-Arg Constructor                   //Empty constructor, but we have to define it
        1.3.3. Parameterized Constructor            //Constructor with parameters, but we have to define it
        1.3.4. Copy Constructor                     //Constructor which copies the values of one object into another object
            1.3.4.1. Shallow Copy                       //Default copy constructor, which copies the values of one object into another object by reference (i.e. address)
            1.3.4.2. Deep Copy                          //Copy constructor, which copies the values of one object into another object by value (i.e. data)
            1.3.4.3. Cloning                            //Alternative of copy constructor, which copies the values of one object into another object by value (i.e. data) by using clone() method. It is faster than copy constructor.
        1.3.6. Constructor Telescoping                 //Calling one constructor from another constructor within the same class, using this() keyword.
        1.3.6. Constructor Overloading              //Having multiple constructors with different parameters
    1.4. Destructor                         //Special type of method which is used to destroy the object. Java doesn't support destructor, but we can use finalize() method to perform the same task.
        1.4.1. finalize() method                    //It is used to perform clean up processing just before object is garbage collected.
    1.5. Inner Class                        //Class within another class, which is used to group classes that belong together, which makes the code more readable and maintainable. There are four types of inner classes:
        1.5.1. Static Inner Class                   //Class within another class, which is declared as static. It cannot access non-static data members and methods. It can be accessed by outer class name.
        1.5.2. Method Local Inner Class             //Class within a method, which is declared inside a method. It cannot access non-final local variable in its enclosing scope. It can be accessed within the method only.
        1.5.3. Anonymous Inner Class                //Class without a name, which is declared and instantiated at the same time. It can be used to override method of a class or an interface. It can be accessed within the method only.
        1.5.4. Nested Inner Class                   //Class within another class, which is declared as non-static. It can access all data members and methods of outer class. It can be accessed by outer class object.
2. Access Modifiers                         //It is used to restrict the access of a class, constructor, data member and method in another class. There are four types of access modifiers:
    2.1. Access Modifiers in terms of Class, Method, Variable, Constructor
        2.1.1. private                          //It can be accessed within the class only.
        2.1.2. protected                        //It can be accessed within the class and its subclasses only.
        2.1.3. public                           //It can be accessed from anywhere.
        2.1.4. default (package protected)      //It can be accessed within the class and its package only.
    2.2. Getter and Setter Methods          //It is used to get and set the values of private data members.
3. this keyword                     //It is used to refer current class instance variable.
    3.1. this() method              //It is used to invoke current class constructor. (Constructor Telescoping)
4. static keyword                   //It is used to create static entities. There are four types of static entities:
    4.1. static variable                    //It is used to create static variable, which belongs to the class rather than object. It can be accessed by class name. Used to create constant variable.
    4.2. static method                      //It is used to create static method, which belongs to the class rather than object. It can be accessed by class name. Used to create utility method.
    4.3. static block                       //It is used to initialize the static data member. It is executed before main method at the time of classloading. It can be used to perform some common tasks such as database connection, etc.
    4.4. static class                       //It is used to create static class, which belongs to the class rather than object. It can be accessed by class name. Used to create nested static class.
5. final keyword                    //It is used to create final entities. There are three types of final entities:
    5.1. final variable                     //It is used to create final variable, which cannot be changed. It can be initialized at the time of declaration or in constructor only.
    5.2. final method                       //It is used to create final method, which cannot be overridden.
    5.3. final class                        //It is used to create final class, which cannot be inherited.
6. new keyword                      //It is used to create object.
    6.1. Memory Allocation                   //It is used to allocate memory to an object.
7. return keyword                   //It is used to return the value from a method.
    7.1. return statement                   //It is used to return the value from a method.
    7.2. return type                        //It is used to specify the type of value that a method returns.
        7.2.1. void                             //It is used to specify that a method doesn't return any value.
        7.2.2. primitive data type              //It is used to specify that a method returns a value of primitive data type.
        7.2.3. class type                       //It is used to specify that a method returns a value of class type.
8. main method                      //It is used to start the execution of program.
9. Strings[] args                   //It is used to accept command line arguments.