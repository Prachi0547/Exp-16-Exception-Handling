# Exp-16-Exception-Handling
# Aim
Write a c++ program:
1. To get a customized error for entering a negative number.
2. To get a customized error for entering a year less than 2000.
# Software Used
VS Code and c++ online compiler.
# Theory
Exception handling in C++ is a mechanism that allows programmers to respond to runtime errors or exceptional conditions in a controlled manner. This feature enables developers to manage errors gracefully, enhancing program robustness and maintainability.

Exception handling in C++ is a powerful feature that allows developers to manage errors in a structured way. By using try, catch, and throw, programmers can separate normal code from error handling, making their applications more robust and easier to maintain.

# Program Code
```
//Negative number error

# include<iostream>
using namespace std;
 int main()
 {  float a;
    cout<< "Enter a positive  numbers: "<<endl;
    cin>>a;

try {
    if ( a<0)
    {
        throw a;
    }
else {
 cout<< "The number  is: "<<a<<endl;
 }
}
catch (const float n)
{
    cout<<"You entered " <<a<<" which is a negative number "<<n;
}
 }
```
```
//Year less than 2000 error

# include<iostream>
using namespace std;
 int main()
 { int year;
    cout << "Enter year greater than 2000: "<<endl;
    cin>>year;

    try{
if ( year<2000)
{
    throw "You entered a year less than 2000";
}
else{
    cout<< "Entered year is: "<<year<<endl;
}
    }
    catch ( const char*msg)

    { 
        cout << msg;

    }
 }
```

# Output
### Negative number error
![image](https://github.com/user-attachments/assets/583b4899-c332-4b08-8da5-00f7e908f792)
![image](https://github.com/user-attachments/assets/8ea92604-a38e-4640-9ed5-740654ef0f07)
### Year less than 2000 error
![image](https://github.com/user-attachments/assets/6380ccdd-d1a3-4828-a835-7271b884da52)
![image](https://github.com/user-attachments/assets/375b67ca-6e79-4bc7-89d0-1b80283bda25)

# Conclusion
We learnt how to use exception handling in c++.
