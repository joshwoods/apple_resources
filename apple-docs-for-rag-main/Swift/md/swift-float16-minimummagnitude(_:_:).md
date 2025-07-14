

- Swift
- Float16
-  minimumMagnitude(\_:\_:) 

Type Method

# minimumMagnitude(\_:\_:)

Returns the value with lesser magnitude.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func minimumMagnitude(
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

Whichever of `x` or `y` has lesser magnitude, or whichever is a number if the other is NaN.

## Discussion

This method returns the value with lesser magnitude of the two given values, preserving order and eliminating NaN when possible. For two values `x` and `y`, the result of `minimumMagnitude(x, y)` is `x` if `x.magnitude 

```
Double.minimumMagnitude(10.0, -25.0)
// 10.0
Double.minimumMagnitude(10.0, .nan)
// 10.0
Double.minimumMagnitude(.nan, -25.0)
// -25.0
Double.minimumMagnitude(.nan, .nan)
// nan
```

The `minimumMagnitude` method implements the `minNumMag` operation defined by the IEEE 754 specification.

