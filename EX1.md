# Ex.No:1
# Ex.Name: Write a CPP Program for Class conversion that can be achieved by conversion function which is done by the use of operator overloading (use double data).

## Aim:
To write a CPP Program for Class conversion that can be achieved by conversion function which is done by the use of operator overloading (use double data)

## Algorithm:
1. Start the program.
2. Define a class containing a double data member.
3. Initialize the data using a constructor.
4. Overload the conversion operator operator double() to return the double value.
5. In main(), create an object of the class.
6. Assign the object to a double variable (conversion happens).
7. Display the converted value.
8. End the program.

## Program:
```
#include <bits/stdc++.h>
#include <string.h>
using namespace std;
class Class_type_one 
{
   float a;
   public:
      Class_type_one()
      {
       cin>>a;
      }
      float get_string()
      {
       return (a);
      }
   void display()
   {
      cout<<a<<endl;
   }
};
class Class_type_two 
{
   float b;
   public:
   Class_type_two()
     {
        
     }
  
    Class_type_two (Class_type_one& a)
    {
       b=a.get_string();
    }
   void display()
   {
      cout<<b;
   }
};
int main()
{
  Class_type_one a1;
  Class_type_two a2;
  a2=a1;
  a1.display();
  a2.display();
   return 0;
}
```


## Output:
<img width="1144" height="278" alt="Screenshot 2025-09-20 173651" src="https://github.com/user-attachments/assets/4f921159-3d40-4530-8a6a-0f4c57b0fbba" />

## Result:
The program successfully demonstrates Class conversion that can be achieved by conversion function which is done by the use of operator overloading.
