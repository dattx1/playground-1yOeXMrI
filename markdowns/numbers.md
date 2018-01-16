# Numeric types in C#

C# offers multiple numeric types, for integer data types and non-integer data types.

**Integer Data Types**

| Type | Description | Minimum Value | Maximum Value |
|------|-------------|---------------|---------------|
| `byte` | Unsigned byte | 0 | 255 |
| `sbyte` | Signed byte | -128 | 127 |
| `short` | Signed byte | -32 768 | 32 767 |
| `ushort` | Unsigned byte | 0 | 65 535 |
| `int` | Signed byte | -2 147 483 648 | 2 147 483 647 |
| `uint` | Unsigned byte | 0 | 4 294 967 295 |
| `long` | Signed byte | -9x10<sup>8</sup> | 9x10<sup>8</sup> |
| `ulong` | Unsigned byte | 0 | 1,8x10<sup>19</sup> |


```C# runnable
// { autofold
using System;

class Hello 
{
    static void Main() 
    {
// }

Console.WriteLine("Hello World!");

// { autofold
    }
}
// }
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced C# template](https://tech.io/select-repo/386)
