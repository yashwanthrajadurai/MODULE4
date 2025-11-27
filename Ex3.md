# Ex.No:3
# Ex.Name: Write a CPP program to show how the override works using virtual functions and how it works without the virtual concept.

## Aim:
To write a CPP program to show how the override works using virtual functions and how it works without the virtual concept.

## Algorithm:
1. Start the program.
2. Create a base class with normal and virtual functions.
3. Create a derived class overriding both functions.
4. Use a base class pointer to point to derived object.
5. Call the normal function → base class version executes.
6. Call the virtual function → derived class version executes.
7. End the program.
   
## Program:
```
#include<iostream>
using namespace std;

class base {
    public:
    string a;
    virtual void disp()
    {
        cin>>a;
        cout<<a<<" Base Class Not overridden"<<endl;
    }
    void display()
    {
        cin>>a;
        cout<<a<<" Base Class Not overridden"<<endl;
    }
};
 
class derived : public base {
   public:
    string a;
    void disp()
    {
        cin>>a;
        cout<<a<<" Derived Class Overridding"<<endl;
    }
    void display()
    {
        cin>>a;
        cout<<a<<" Derived Class Overridding"<<endl;
    }
};
 
int main()
{
    //Base Class Pointer
    base *ptr;
    //Derived Class Object
    derived obj;
    //Assign Base Class Pointer with Derived class Object
    ptr = &obj;
    ptr->disp();
    ptr->display();
    // Virtual function, binded at runtime
    
    // Non-virtual function, binded at compile time
    
   
    return 0;
}
```


## Output:
<img width="922" height="357" alt="Screenshot 2025-09-20 174408" src="https://github.com/user-attachments/assets/8d46ca68-208c-4154-9061-68c2b663fab5" />

## Result:
The program successfully demonstrates how the override works using virtual functions and how it works without the virtual concept.
