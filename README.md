Toy-C-Compiler-Frontend
====
A Compiler front end to produce code for llvm backend

## Introduction

* This is a toy-project to build an easy C Compiler frontend
* Develop using TDD
* Using standard C++11
* Will Support cross-platform

## Plan

Here is the plan of this toy-project

- [ ] Write testcases for the project
- [ ] 

## How to contribute

* Just make Pull Request ~
 * the commit format is : "codemodulename: What you do"
 
  > For example , you add A function foo into the grammer anaylze module then your commit should
   look like this : grammar anaylze: Add function foo XXXXXXXXXXXXX
* Be aware of the code styling , see the sample code to make sure you obey the code styling

Sample Code : [link](http://geosoft.no/development/cppstyle.html)
```C++

    // Coding Style Guide
    // Based on http://geosoft.no/development/cppstyle.html

    // NO tabs! Only space. Tabs are 4 spaces wide.

    // All names should be written in English.
    // NOT: bestandsNaam;
    fileName;

    // Class names are writen with CamelCasing starting with a capital
    // File names shoud match there class names. "ClassName.cpp", NOT: "class_name.cpp"
    class ClassName {

    };

    // A class with a word like "HTML" is also written with CamelCasing
    // NOT: exportHTMLSource();
    class ExportHtmlSource {

    };

    // Private class variables should start with an underscore suffix.
    // In general, the use of global variables should be avoided.
    class SomeClass {
        public:
            int width;

        protected:
            int height;
            
        private:
            int _length;
    };

    // If-else statements
    if (a < b)
    {
        doStuffFunction();
    }

    // Mulit line if-else
    if (a > b) 
    {
        testFunction();
    } 
    else if (a > c) 
    {
        basicFunction();
    } 
    else 
    {
        debug();
    }

    // For oneline if statements short version is allowed
    if (a > b)
        doThisFunction(c); 

    // For loop. Use i, j, k, etc for iterator variables
    // Variables named j, k etc. should be used for nested loops only.
    for (int i=0; i<10; i++) 
    {
        doStuff();
    }

    // Complex conditional expressions must be avoided. Introduce temporary boolean variables instead
    bool isFinished         = (elementNo < 0) || (elementNo > maxElement);
    bool isRepeatedEntry    = elementNo == lastElement;
    if (isFinished || isRepeatedEntry) 
    {
        doSomethingCool();
    }

    // Defining functions using camelCase with small starting character
    // Use a "_" after the attribute variables to show there are attributes
    // Like class namings stuff like "HTML" is written as "Html". NOT: thisHTMLIsMyFunctionName
    void setPlayerPosition(int x_,int y_,int z_ ) 
    {
        playerPosition.set(x_, y_, z_);
    }

    bool thisHtmlIsGood()
    {
        return true;
    }

    // If a function is called in de code make sure there a spaces between the "(", ")" and ","
    thisIsMyFunctionName( mouseX, mouseY, mouseZ );

    // Names representing namespaces should be all lowercase.
    model::analyzer, io::iomanager, common::math::geometry

    // Names representing types must be in mixed case starting with upper case.
    Line, SavingsAccount

    // Variable names must be in mixed case starting with lower case
    line, savingsAccount

    // Variables with a large scope should have long names, variables with a small scope can have short names 
    x, y, z
    posX, posY, posZ

    // Constants are written with all capitals and words are seperated with underscores
    // In general, the use of such constants should be minimized.
    #define THIS_IS_A_CONSTANT 11500

    // The name of the object is implicit, and should be avoided in a method name.
    // NOT: line.getLineLength();
    line.getLength();

    // Plural form should be used on names representing a collection of objects.
    vector<Point>  points;
    int            values[];

    // The prefix n should be used for variables representing a number of objects.
    nPoints, nLines

    // The suffix No should be used for variables representing an entity number.
    tableNo, employeeNo

    // Variables representing GUI components should be suffixed by the component type name.
    mainWindow, propertiesDialog, widthScale, loginText, leftScrollbar, 
    mainForm, fileMenu, minLabel, exitButton, yesToggle;

    // The prefix is should be used for boolean variables and methods.
    // Negated boolean variable names must be avoided. Example "isError", NOT: "isNoError".
    isSet, isVisible, isFinished, isFound, isOpen

    // There are a few alternatives to the is prefix that fit better in some situations. 
    // These are the has, can and should prefixes:
    bool hasLicense();
    bool canEvaluate();
    bool shouldSort();

    // Floating point constants should always be written with decimal point and at least one decimal.
    // NOT: double total = 0;
    float total = 1.0;

    // Complement names must be used for complement operations
    // Examples: get/set, add/remove, create/destroy, start/stop, insert/delete,
    // increment/decrement, old/new, begin/end, first/last, up/down, min/max,
    // next/previous, old/new, open/close, show/hide, suspend/resume, etc.

    // Abbreviations in names should be avoided.
    // NOT: compAvg();
    // Examples: never write "cmd" instead of "command" or "cp" instead of "copy"
    computeAverage();

    // Group variables by type
    int     x;
    int     y;
    int     z;

    char    a;
    char    b

    bool    isBool;

    // The terms get/set must be used where an attribute is accessed directly.
    employee.getName();
    employee.setName( name );

    // The term find can be used in methods where something is looked up.
    vertex.findNearestVertex();

    // The term initialize can be used where an object or a concept is established.
    // The american initialize should be preferred over the English initialise. Abbreviation init should be avoided.
    printer.initializeFontSet();

    // Structs are named the same way as classes
    struct Stop 
    {
        string name;
    };

    // Vector lists, for example a struct or class, should be writen like:
    vector<Stop> stops;

    // Use appropiate variable types
    // http://www.tutorialspoint.com/cplusplus/cpp_data_types.htm
    // signed char          : -127 to 127 (note, not -128 to 127; this accommodates 1s-complement platforms)
    // unsigned char        : 0 to 255
    // char                 : -127 to 127 or 0 to 255 (depends on default char signedness)
    // signed short         : -32767 to 32767
    // unsigned short       : 0 to 65535
    // signed int           : -32767 to 32767
    // unsigned int         : 0 to 65535
    // signed long          : -2147483647 to 2147483647
    // unsigned long        : 0 to 4294967295
    // signed long long     : -9223372036854775807 to 9223372036854775807
    // unsigned long long   : 0 to 18446744073709551615

    // Exception statements
    try {
        trySomething();
    }
    catch( ExceptionName e ) {
        cout << "[exception] " << e << endl;
    }



```



