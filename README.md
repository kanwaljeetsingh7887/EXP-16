# EXP-15

## Aim:
**To study and implement Exception Handling in C++.**

## Software:
`Microsoft VSCode`

## Theory:
<ul>
    <li>In C++ exceptions are runtime anomalies or abnormal conditions that a program encounters durig its execution. </li>
    <li>The process of handling these exceptions is known as exception handling. </li> 
    <li>Using the exception handling mechanism, the control from one part of the program where the exception occurred can be transferred to another part of the 
   code.</li>
    <li>It can be done using three keywords: <ol>
        <li>try - The try keyword represents a block of code that may throw an exception placed inside the try block. It’s followed by one or more catch blocks. If an exception occurs, try block throws that exception.</li>
        <li>catch - The catch statement represents a block of code that is executed when a particular exception is thrown from the try block. The code to handle the exception is written inside the catch block.</li>
        <li>throw - An exception in C++ can be thrown using the throw keyword. When a program encounters a throw statement, then it immediately terminates the current function and starts finding a matching catch block to handle the thrown exception.</li></ol></li>
</ul>

}
## Code: 16A
(A) <br> 
```cpp
// NAME - Kanwaljeet singh
//PRN - 23070123124 
// EXPERIMET - 16(A) 

// EXCEPTION HANDLING 

#include<iostream>
using namespace std;

int main()
{
    float n1, n2, n3, n4, ans;
    cout<<"Enter values of numbers 1 and 2: ";
    cin>>n1>>n2;
    try{
        if(n2==0) {
            throw n2;
        }
        else {
            ans=n1/n2;
            cout<<"Answer = "<<ans<<endl;
        }
    }
    catch(float num) {
        cout<<"\n ERROR: Division by "<<num<<endl;
    }
}
```

## Output:
![image](https://github.com/user-attachments/assets/4722642c-c087-4388-9b39-c5ba3d50f5de)







## Code: 15B
 <br> 
```cpp
// NAME - RIDDHI LOKHANDE
// PRN - 23070123107
// EXPERIMENT - 16(B) 

// EXCEPTION HANDLING 

#include<iostream>
using namespace std;

int main()
{
    int age;
    cout<<"Enter age: ";
    cin>>age;
    try{
        if(age<18) {
            throw age;
        }
        else {
            cout<<"Age: "<<age<<"\n APPROVED"<<endl;
        }
    }
    catch(int a) {
        cout<<"\n ERROR: Underage! ("<<age<<")"<<endl;
    }
}

```
## Output:
![image](https://github.com/user-attachments/assets/7ca1f640-6ed1-4582-bdaf-af329dd0d4de)





## Code: 15C
```cpp
// NAME - Kanwaljeet singh
// PRN - 23070123124
// EXPERIMENT - 15(C)
#include<iostream>
using namespace std;      

// Creating function. 
void reverse(char *str)
{
    if(*str)  // Base Condition 
    {
        reverse(str+1);  // Recursion 
        cout<<("%c",*str);
    }
}

int main() 
{
    char a[50];
    cout<<"Enter a string: ";
    cin>>a;
    reverse(a);  // Function calling 
    return 0; 
}       
```
## Output:
![image](https://github.com/user-attachments/assets/f4560189-5057-4d13-984f-a286c27dfbbd)



## Code: 15D
```cpp
// NAME - Kanwaljeet singh
// PRN - 23070123124
// EXPERIMENT - 14(D)

#include<iostream> 
using namespace std;

// Creating a function 

void print_rev(int i){
    if(i>0)          // Base Condition  
    {
        cout<<(i%10);
        print_rev(i/10);   // Recursion 
    }
}

int main()
{
    int i;
    cout<<"Enter the number: ";
    cin>>i;
    print_rev(i);  // Function Calling   
    return 0;
}           
```                  
## Output:
![image](https://github.com/user-attachments/assets/31f30dd0-ee45-4c5d-8bcd-118cd2145e45)




### Conclusion:
I learnt about Exception Handling in C++ and about its three keywords: try, catch and throw. 
