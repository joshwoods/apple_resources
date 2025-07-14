

- Swift
- Float
-  sign 

Instance Property

# sign

The sign of the floating-point value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var sign: FloatingPointSign { get }
```

## Discussion

The `sign` property is `.minus` if the value’s signbit is set, and `.plus` otherwise. For example:

```
let x = -33.375
// x.sign == .minus
```

Don’t use this property to check whether a floating point value is negative. For a value `x`, the comparison `x.sign == .minus` is not necessarily the same as `x 

## See Also

### Finding the Sign and Magnitude

var magnitude: Float

The magnitude of this value.

typealias Magnitude

A type that can represent the absolute value of any possible value of the conforming type.

