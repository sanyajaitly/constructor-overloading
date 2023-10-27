# constructor-overloading

AIM

Constructors-Overloading

THEORY 


To understand constructor overloading in C++, we first need to understand what constructors are. When we create a class object, the constructors are unique methods that are automatically invoked. We use constructors to initialize valid values to an object's data members. In C++, we can have many constructors in the same class as long as they all have a different list of arguments. This concept is called Constructor Overloading and is quite similar to function overloading. A constructor is called depending on how many and what kind of arguments are passed.

Types of Constructors

There are three types of constructors.

Default Constructor
The constructor that does not take any argument or all the arguments it takes are default variables and is referred to as the default constructor. It does not have function parameters. It is also known as a zero-argument constructor.

Syntax

class ClassName

{

public:

ClassName()// Default constructor

{ .... }

// Other member functions.

};

2.Parameterized Constructor

A constructor which has parameters are known as parameterized constructor. In contrast to the default constructor, it has parameters (or arguments) in the constructor definition and declaration. Multiple arguments can also pass through a parameterized constructor. This type of constructor is frequently used for overloading and initializing multiple data elements of objects with different initial values.

Syntax

class ClassName

{

public:

ClassName(data_type variable) // Parameterized constructor.

{ .... }

// Other member functions.

};

Copy Constructor
Constructors in which we initialize the class object using another object of the same class is called copy constructor. It is used to initialize the members of a newly created object by copying the members of an already existing object.

Syntax

class ClassName

{ public: ClassName(const ClassName & old_object) // Copy constructor.

{
    ....
}

// Other member functions.

};


ALGORITHM 


Part-A

Constructor Overloading Algorithm:

1.Start

2.Define a class with multiple constructor declarations, each with a different parameter list. These constructors may have different numbers or types of parameters.

3.Inside each constructor, initialize the object's member variables using the provided arguments.

4.Optionally, perform any necessary initialization or validation logic inside the constructors.

5.Create objects of the class by specifying different sets of arguments when invoking the constructors.

6.When creating an object, the compiler will determine which constructor to call based on the number and types of arguments provided.

7.Use the objects to access member variables and member functions as needed.

8.End

Part-B
1.Include the necessary header file for input and output (iostream).

2.Declare a class named area.

3.Inside the area class, declare two private member variables length and width, both of type float.

4.Define a default constructor for the area class:

5.Initialize the length member variable to 10.

6.Initialize the width member variable to 20.

7.Calculate the area (ar) as the product of length and width.

8.Display a message indicating the area of the room using cout.

9.Define a parameterized constructor for the area class that takes two float arguments (l and b):

10.Initialize the length member variable with the value of l.

11.Initialize the width member variable with the value of b.

12.Calculate the area (ar) as the product of length and width.

13.Display a message indicating the area of the room using cout.

14.In the main function:

15.Create three objects of the area class (A1, A2, and A3) using different constructors.

16.For A1, the default constructor is used, which sets length to 10 and width to 20, and calculates the area based on these values.

17.For A2, a parameterized constructor is used with the arguments 11.52 and 20. It sets length to 11.52 and width to 20 and calculates the area accordingly.

18.For A3, a parameterized constructor is used with the arguments 15.20 and 20.20. It sets length to 15.20 and width to 20.20 and calculates the area based on these values.

19.Return 0 to indicate successful program termination.

20.This code defines a class for calculating and displaying the area of a room, providing both default and parameterized constructors for flexibility in specifying the room's dimensions.

Part-C
1.Include the necessary header file for input and output (iostream).

2.Declare a class named construct.

3.Inside the construct class, declare two integer member variables a and b.

4.Define a default constructor for the construct class:

5.Initialize a to 10.

6.Print the value of a using cout.

7.Define a constructor that takes one integer argument x for the construct class:

8.Set the member variable a to 29.

9.Print the value of x using cout.

10.Define a constructor that takes two integer arguments a_val and b_val for the construct class:

11.Set the member variables a and b to the values of a_val and b_val, respectively.

12.Print the values of a and b using cout.

13.Define a constructor that takes one integer argument a_val and one float argument b_val for the construct class:

14.Set the member variable a to the value of a_val.

15.Print the value of a using cout.

16.Print the value of b_val using cout.

17.In the main function:

18.Create four objects of the construct class (obj1, obj2, obj3, and obj4) using different constructors.

19.Display the values of a and b for each object using the cout statements within the constructors.

20.Return 0 to indicate successful program termination.

This code demonstrates the use of constructors with different parameter sets and creates objects of the construct class to showcase their behavior. Depending on the constructor used, it initializes and displays values of the member variables a and b in various ways.
