

- Swift
- Float80
-  maximumMagnitude(\_:\_:) 

Type Method

# maximumMagnitude(\_:\_:)

Returns the value with greater magnitude.

macOS 10.10+

``` source
static func maximumMagnitude(
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

Whichever of `x` or `y` has greater magnitude, or whichever is a number if the other is NaN.

## Discussion

This method returns the value with greater magnitude of the two given values, preserving order and eliminating NaN when possible. For two values `x` and `y`, the result of `maximumMagnitude(x, y)` is `x` if `x.magnitude > y.magnitude`, `y` if `x.magnitude 

```
Double.maximumMagnitude(10.0, -25.0)
// -25.0
Double.maximumMagnitude(10.0, .nan)
// 10.0
Double.maximumMagnitude(.nan, -25.0)
// -25.0
Double.maximumMagnitude(.nan, .nan)
// nan
```

The `maximumMagnitude` method implements the `maxNumMag` operation defined by the IEEE 754 specification.

