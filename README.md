# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
 ##Algorithm:
 
 
 
 ##Program:
 ```
 using System;

namespace ConsoleApp8
{
    class example
    {
        public int length;
        public example()
        {
            length = 10;
        }
        public example(int i)
        {
            length = i;
        }
        public static bool operator == (example obj1, example obj2)
        {

            return obj1.Equals(obj2);
        }
        public static bool operator != (example obj1, example obj2)
        {
           return !obj1.Equals(obj2);
        }
        public static void Main()
        {
            example e1 = new example();
            example e2 = new example(20);
            example e3 = new example();
            example e4 = e3;
            if (e1 == e2)
            {
                Console.WriteLine("Equal");
            }
            else if (e1 != e2)
            {
                Console.WriteLine("Not equal");
            }
        }
    }
}

```
 
 ##Output:
 ![ahakjkre](https://user-images.githubusercontent.com/75235212/198813608-8dca83b3-d28e-4adf-a571-d5cd92895cd6.PNG)

 
 ##Result:
Experiment has been successfully executed
