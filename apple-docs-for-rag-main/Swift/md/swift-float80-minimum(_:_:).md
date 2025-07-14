

- Swift
- Float80
-  minimum(\_:\_:) 

Type Method

# minimum(\_:\_:)

Returns the lesser of the two given values.

macOS 10.10+

``` source
static func minimum(
    _ x: Self,
    _ y: Self
) -> Self
```

## Parameters 

`x`  

A floating-point value.

`y`  

Another floating-point value.

## Return Value

The minimum of `x` and `y`, or whichever is a number if the other is NaN.

## Discussion

This method returns the minimum of two values, preserving order and eliminating NaN when possible. For two values `x` and `y`, the result of `minimum(x, y)` is `x` if `x 

```
Double.minimum(10.0, -25.0)
// -25.0
Double.minimum(10.0, .nan)
// 10.0
Double.minimum(.nan, -25.0)
// -25.0
Double.minimum(.nan, .nan)
// nan
```

The `minimum` method implements the `minNum` operation defined by the IEEE 754 specification.

