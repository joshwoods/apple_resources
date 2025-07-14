

- ImageCaptureCore
- ICReturnPTPDeviceError
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether two values are not equal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.2+macOS 10.9+visionOS 1.0+Xcode 11.2+

``` source
static func != (lhs: ICReturnPTPDeviceError, rhs: ICReturnPTPDeviceError) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Inequality is the inverse of equality. For any values `a` and `b`, `a != b` implies that `a == b` is `false`.

This is the default implementation of the not-equal-to operator (`!=`) for any type that conforms to `Equatable`.

