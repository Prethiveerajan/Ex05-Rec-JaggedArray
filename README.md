# Ex05-Rec-JaggedArray
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
## Step1:
Start.

## Step2:
Create a jagged array of 4arrays.

int[][] array = new int[4][];

## Step3:
Give the sample CPU usage in the jagged array.

## Step4:
Print the sample CPU usage in the jagged array.

## Step5:
stop.


## Program:
```
using System;
using System.Globalization;

namespace console
{
    class programm
    {
        static void Main(string[] args)
        {
            int[][] array = new int[4][];
            array[0] = new int[4];
            array[1] = new int[3];
            array[2] = new int[2];
            array[3] = new int[5];
            for (int i = 0; i < array.Length; i++)
            {
                for (int j = 0; j < array[i].Length; j++)
                {
                    array[i][j] = i * j + 70;

                }
            }
            for (int i = 0; i < array.Length; i++)
            {
                for (int j = 0; j < array[i].Length; j++)
                {
                    Console.WriteLine("CPU USAGE IN NODE {0}IS {1}%", i, array[i][j]);
                }
            }
            Console.WriteLine();
        }
    }
}   


```
## Output:
![output](op1.png)

## Result:
Thus,C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is executed successfully
