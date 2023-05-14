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

</br></br> </br>
 
 ## Program:
 Developed By: Senthil Kumar S
 </br>
 Register No.: 212221230091
 ```c#
using System;

namespace OperatorOverloading
{
    class program
    {
        public int p1, p2;

        public program()
        {
            p1 = 70;
            p2 = 69;
        }
        public program(int p3, int p4)
        {
            p1 = p3;
            p2 = p4;
        }
        public static bool operator ==(program p1, program p2)
        {
            return p1.Equals(p2);
        }
        public static bool operator !=(program p1, program p2)
        {
            return !(p1 == p2);
        }
        public static void Main()
        {
            program o1 = new program();
            program o2 = new program(75, 65);

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
![random](https://github.com/Senthil-Kumar-710/demo/assets/93860256/dc9d114f-7007-407f-8eaa-f72629f07e57)


 
 ## Result:
Thus, a C# program to find the volume of a box using operator overloading is implemented successfully.
