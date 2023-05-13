# <p align="center">Operator-Overloading</p>


## Aim:
To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
## Algorithm:
### Step1:
Create a class named program.
### Step 2:
Create two constructors with different arguments to implement operator overloading
### Step 3:
Create boolean operators to check equals and not equal condition and to implement operator overloading.
### Step 4:
Create a Main function
### Step 5:
Create two objects. One without arguments & the other with arguments
### Step 6:
Check whether the objects are equal or not using if-else condition

</br> </br> </br> </br></br> </br>
 
 ## Program:
 Developed By: **Shafeeq Ahamed.S**
 </br>
 Register No.: **212221230092**
 ```c#
using System;

namespace OperatorOverloading
{
    class program
    {
        public int p1, p2;
        
        public program()
        {
            p1 = 10;
            p2 = 15;
        }
        public program(int p3, int p4)
        {
            p1 = p3;
            p2 = p4;
        }
        public static bool operator == (program p1, program p2)
        {
            return p1.Equals(p2);
        }
        public static bool operator != (program p1, program p2)
        {
            return !(p1 == p2);
        }
        public static void Main()
        {
            program o1 = new program();
            program o2 = new program(15,30);

            Console.WriteLine("Object P1: {0} {1}", o1.p1, o1.p2);
            Console.WriteLine("Object P2: {0} {1}", o2.p1, o2.p2);

            if (o1 == o2)
                Console.WriteLine("Objects are equal");

            else if (o1 != o2)
                Console.WriteLine("Objects are not equal");
        }
    }
}
 ```
 
 </br>
 
 
 ## Output:
![image](https://github.com/ShafeeqAhamedS/C-_Exp_6_Operator-Overloading/assets/93427237/67fe790f-3757-4473-b97e-9272bea90e20)

 
 ## Result:
Thus, a C# program to find the volume of a box using operator overloading is implemented successfully.
