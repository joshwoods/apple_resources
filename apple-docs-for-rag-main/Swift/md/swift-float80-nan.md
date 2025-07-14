

- Swift
- Float80
-  nan 

Type Property

# nan

A quiet NaN (“not a number”).

macOS 10.10+

``` source
static var nan: Float80 { get }
```

## Discussion

A NaN compares not equal, not greater than, and not less than every value, including itself. Passing a NaN to an operation generally results in NaN.

```
let x = 1.21
// x > Double.nan == false
// x 

Because a NaN always compares not equal to itself, to test whether a floating-point value is NaN, use its `isNaN` property instead of the equal-to operator (`==`). In the following example, `y` is NaN.

```
let y = x + Double.nan
print(y == Double.nan)
// Prints "false"
print(y.isNaN)
// Prints "true"
```

