using System;
using System.Collections.Generic;
using System.Linq;

class Program
{
    static void Main()
    {
        List<int> numbers = GenerateRandomNumbers(10, 1, 100);
        Console.WriteLine("Random Numbers: " + string.Join(", ", numbers));
        Console.WriteLine("Fibonacci Sequence: " + string.Join(", ", Fibonacci(10)));
        Console.WriteLine("Is 17 Prime? " + IsPrime(17));
        Console.WriteLine("Reversed String: " + ReverseString("Hello World"));
        Console.WriteLine("Factorial of 5: " + Factorial(5));
        Console.WriteLine("Sorted Numbers: " + string.Join(", ", numbers.OrderBy(n => n)));
    }

    static List<int> GenerateRandomNumbers(int count, int min, int max)
    {
        Random rand = new Random();
        List<int> numbers = new List<int>();
        for (int i = 0; i < count; i++)
        {
            numbers.Add(rand.Next(min, max + 1));
        }
        return numbers;
    }

    static List<int> Fibonacci(int n)
    {
        List<int> sequence = new List<int> { 0, 1 };
        for (int i = 2; i < n; i++)
        {
            sequence.Add(sequence[i - 1] + sequence[i - 2]);
        }
        return sequence;
    }

    static bool IsPrime(int num)
    {
        if (num < 2) return false;
        for (int i = 2; i <= Math.Sqrt(num); i++)
        {
            if (num % i == 0) return false;
        }
        return true;
    }

    static string ReverseString(string str)
    {
        char[] charArray = str.ToCharArray();
        Array.Reverse(charArray);
        return new string(charArray);
    }

    static int Factorial(int n)
    {
        if (n == 0) return 1;
        return n * Factorial(n - 1);
    }
}
