# Ex.No:5
# Ex.Name: Write A CPP program to Demonstrate on the object delegation (use float data)

## Aim:
To write A CPP program to Demonstrate on the object delegation (use float data).

## Algorithm:
1. Start the program.
2. Create a helper class with float data and a function to display it.
3. Create a main class that contains an object of the helper class.
4. Delegate task of displaying data to the helper object.
5. In main(), create object of the main class.
6. Call the function → delegated helper function executes.
7. End the program.

## Program:
```
// C++ program to illustrate the
// Object Delegation
#include <iostream>
using namespace std;
class First 
{
    
    public:float x;
    First(){
        x = 0.0;
    }
    
    void disp(){
        cout<<x<<endl;
    }
};
class Second 
{
	float y;
	First objF;
	public:
	
	Second(float value)
	{
	    y = value;
	    objF.x = y;
	}
	
	void display()
	{
	    cout<<objF.x<<endl;
	}
};

// Driver Code
int main()
{
	float value;
	cin>>value;
	Second objS(value);
	objS.display();
	return 0;
}
```


## Output:
<img width="495" height="341" alt="Screenshot 2025-09-20 175223" src="https://github.com/user-attachments/assets/bbaf2a1f-ef32-4e48-8f33-4c093e280674" />

## Result:
The program successfully demonstrates Demonstrate on the object delegation (use float data).
