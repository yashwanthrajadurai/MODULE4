# Ex.No:4
# Ex.Name: Write a CPP program to demonstrate on the object composition (use string data).

## Aim:
To Write a CPP program to demonstrate on the object composition (use string data).

## Algorithm:
1. Start the program.
2. Create a class Address with string data.
3. Create another class Person that has an Address object as its member (composition).
4. Initialize both classes using constructors.
5. Display details of Person and Address through a member function.
6. End the program.

## Program:
```
#include <iostream>
using namespace std;
// Simple class
class A 
{
    public:
    string x;
	A(){
	    x="";
	}
	A(string a){
	    cout<<"Constructor A(string a) is invoked"<<endl;
	    x=a;
	}
};
class B 
{
    string b;
    A objA;
    public:
    B(string a) : objA(a){
        b=a;
    }
    void display(){
        cout << "Data in object of class B = " << b<< endl; 
        cout << "Data in member object of class A in class B = " << objA.x; 
    }
};

// Driver code
int main()
{
    string a;
    cin>>a;
	B objb(a);
	objb.display();
	return 0;
}
```


## Output:
<img width="1176" height="366" alt="Screenshot 2025-09-20 174754" src="https://github.com/user-attachments/assets/8234c480-705a-4ac7-ac31-35152685906e" />

## Result:
The program successfully demonstrates demonstrate on the object composition (use string data).
