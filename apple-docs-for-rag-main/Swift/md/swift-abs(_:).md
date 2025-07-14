

- Swift
-  abs(\_:) 

Function

# abs(\_:)

Returns the absolute value of the given number.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func abs(_ x: T) -> T where T : Comparable, T : SignedNumeric
```

## Parameters 

`x`  

A signed number.

## Return Value

The absolute value of `x`.

## Discussion

The absolute value of `x` must be representable in the same type. In particular, the absolute value of a signed, fixed-width integer type’s minimum cannot be represented.

```
let x = Int8.min
// x == -128
let y = abs(x)
// Overflow error
```

## See Also

### Finding the Sign and Magnitude

var magnitude: UInt

The magnitude of this value.

typealias Magnitude

A type that can represent the absolute value of any possible value of this type.

func signum() -> Int

Returns `-1` if this value is negative and `1` if it’s positive; otherwise, `0`.

