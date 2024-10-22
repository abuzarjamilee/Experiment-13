**Experiment 13**

**Aim:**  
To study and implement constructor overloading in C++.

**Apparatus:**  
VS Code, GitHub

**Theory:**  
**Understanding Constructor Overloading in C++:**
1. When an object is instantiated, the C++ compiler identifies the constructor that matches the provided arguments.
2. If no arguments are supplied, the default constructor is invoked.
3. If arguments are given, the constructor that corresponds to the argument list is called.

**Rules for Constructor Overloading in C++:**
1. **Different Signatures:** Each overloaded constructor must have a unique signature (i.e., a different set of parameters).
2. **No Return Type:** Overloaded constructors do not have a return type, not even `void`.
3. **Same Name:** All constructors must have the same name as the class.

**Characteristics of Constructor Overloading:**
1. **Multiple Constructors:** A class can have multiple constructors, each with different parameters.
2. **Different Parameter Lists:** Constructors can differ in the number, type, or order of parameters.
3. **Automatic Selection:** The compiler automatically selects the appropriate constructor during object instantiation.
4. **Flexible Initialization:** Overloaded constructors provide various ways to initialize an object based on available data.
5. **Same Name:** All constructors share the same name as the class.
6. **No Return Type:** Like any constructor, overloaded constructors do not have a return type.
7. **Enhanced Versatility:** Constructor overloading increases the flexibility of object creation.

**Advantages of Constructor Overloading in C++:**
1. **Flexibility:** Classes can be instantiated in various ways depending on available data.
2. **Ease of Use:** Users can conveniently initialize objects with different data sets.
3. **Improved Readability:** The code becomes more readable by clearly defining object creation methods.

**Code:**
```cpp
#include <iostream>
using namespace std;

class Room {
private:
    double length, breadth;

public:
    Room() {
        length = 1.2;
        breadth = 2.3;
    }
    
    Room(double len, double bre) {
        length = len;
        breadth = bre;
    }
    
    Room(double len) {
        length = len;
        breadth = 4.5;
    }
    
    double area() {
        return length * breadth;
    }
};

int main() {
    Room r1, r2(6.7, 7.8), r3(9.1);
    cout << "No parameters passed: " << endl;
    cout << "Area: " << r1.area() << endl;
    cout << "Two parameters passed: " << endl;
    cout << "Area: " << r2.area() << endl;
    cout << "One parameter passed: " << endl;
    cout << "Area: " << r3.area() << endl;
}
```
**Output:**  
![image](https://github.com/user-attachments/assets/81833a04-3003-46c8-b6c5-8277b8e32f76)


**Conclusion:**  
This program illustrates the concept of constructor overloading.

--- 

Let me know if you need any further modifications!
