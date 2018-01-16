# Precision & Rounding

Due to the internal representation of `float` and `double` numeric types, arithmetic operations on these types can result in imprecise results, which will be rounded to the nearest _representable_ value.

```C# runnable
// { autofold
using System;

class Example 
{
    static void Main() 
    {
// }
    double a = 0.1;
    double b = 0.01;
    double c = a * a;
    
    // We should have true, as 0,1 * 0,1 = 0,01
    Console.WriteLine($"b == c: {b == c}");
// { autofold
    }
}
// }
```

When using non-integer numeric types in C#, it is important to know the pros and cons of each specific type.
* `float` and `double` types are meant to use when performance is more important than precision.
* `decimal` is instead more accurate than the two others, at the cost of performance. When doing arithmetic operations that require a high precision in results without roundings, make sure you use the `decimal` type (this is even more important when doing calculation about money or finance).

If we use the `decimal` type for the same operation that above, the result is correct.

```C# runnable
// { autofold
using System;

class Example 
{
    static void Main() 
    {
// }
    decimal a = 0.1m;
    decimal b = 0.01m;
    decimal c = a * a;
    
    // We should have true, as 0,1 * 0,1 = 0,01
    Console.WriteLine($"b == c: {b == c}");
// { autofold
    }
}
// }
```