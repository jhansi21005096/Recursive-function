# Recursive-function

##Aim: To write a C# program to reverse a number using recursive function.

## Algorithm:
### Step 1:
Create a function for reversing.

### Step 2:
Get the input from the user.

### Step 3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

### Step 4:
Recrseively calling the function to get the reversed number.

### Step 5:
print the reversed number.
## Program:
```
using recursive;
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace recursive
{
    class program
    {
        int reverse = 0, remainder;
        public int rev(int n)
        {
            remainder = n % 10;
            if (remainder == 0)
            {
                return reverse;
            }
            else
            {
                remainder = n % 10;
                reverse = reverse * 10 + remainder;
                n = n / 10;
                return rev(n);
            }
        }
    }
}
class program1
{
    static void Main(string[] args)
    {
        int n;
        Console.Write("Enter number: ");
        n = Convert.ToInt32(Console.ReadLine());

        program a = new program();
        Console.WriteLine("The revered number = " + a.rev(n));
    }
}
```
## Output:
![output]()
## Result:
To write a C# program to reverse a number using recursive function is executed successfully.
