

- Swift
- Float80
-  +(\_:) 

Operator

# +(\_:)

Returns the given number unchanged.

macOS 10.10+

``` source
static func + (x: Self) -> Self
```

## Return Value

The given argument without any changes.

## Discussion

You can use the unary plus operator (`+`) to provide symmetry in your code for positive numbers when also using the unary minus operator.

```
let x = -21
let y = +21
// x == -21
// y == 21
```

