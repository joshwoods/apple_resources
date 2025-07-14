

- Swift
- Float80
-  sign 

Instance Property

# sign

The sign of the floating-point value.

macOS 10.10+

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

