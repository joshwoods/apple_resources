

- Swift
- FloatingPoint
-  maximum(\_:\_:) 

Type Method

# maximum(\_:\_:)

Returns the greater of the two given values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func maximum(
    _ x: Self,
    _ y: Self
) -> Self
```

**Required** Default implementation provided.

## Parameters 

`x`  

A floating-point value.

`y`  

Another floating-point value.

## Return Value

The greater of `x` and `y`, or whichever is a number if the other is NaN.

## Discussion

This method returns the maximum of two values, preserving order and eliminating NaN when possible. For two values `x` and `y`, the result of `maximum(x, y)` is `x` if `x > y`, `y` if `x 

```
Double.maximum(10.0, -25.0)
// 10.0
Double.maximum(10.0, .nan)
// 10.0
Double.maximum(.nan, -25.0)
// -25.0
Double.maximum(.nan, .nan)
// nan
```

The `maximum` method implements the `maxNum` operation defined by the IEEE 754 specification.

## Default Implementations

### FloatingPoint Implementations

static func maximum(Self, Self) -> Self

Returns the greater of the two given values.

