# Exp-10--Operations-on-Pointers
# AIM

To learn pointer operations in c++.

# Software Used

VS code AND Online Cpp Compiler

# Problem Statement

1.) Write a c++ program to swap the numbers using call by value.

2.) Write a c++ program to swap the numbers using call by reference.

# Theory

Call by value :-

When a function is called, new elements are created on the stack memory to store the essential information about the functions as well as allocated memory space for parameters and the return value.

Call by reference :-

The call by reference method of passing arguments to a function copies the reference of an argument into the formal parameter. Inside the function, the reference is used to access the actual argument used in the call. This means that changes made to the parameter affect the passed argument.

# Problem Codes

```javascript


//CALL BY VALUE
 #include <iostream>
using namespace std;
 void swap(int a,int b)
 
{
    int c;
    c=a;
    a=b;
    b=c;
   cout<<"Inside swabByValue function: "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
}
int main()
 
{ int a=2,b=7;
cout<<"Before swabByValue: "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
swap(a,b);
cout<<"After swapByValue: "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
}

//CALL BY REFERENCE

 #include <iostream>
using namespace std;
 void swap(int *a,int* b)
 
{
    int c;
    c=*a;
    *a=*b;
    *b=c;
  cout<<"Inside swabByReference function: "<<"a = "<< *a<<" , "<<"b = "<< *b<<endl;
    
}
 int main()
 
{ int a=2,b=7;
cout<<"Before swabByReference: "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
swap(&a,&b); 
cout<<"After swapByReference: "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
}

```
# Output
## 1) Call by value
![Exp 10- call by value](https://github.com/user-attachments/assets/11ff0bff-7028-4e35-93f4-271c9a90d326)

## 2) Call by reference
![Exp 10 - call by referance](https://github.com/user-attachments/assets/b25a3484-bd23-4861-9c41-2da648b4912f)

# Conclusion

We learnt to swap the numbers using call by value and call by reference.
