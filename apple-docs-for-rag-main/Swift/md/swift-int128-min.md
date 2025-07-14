

- Swift
- Int128
-  min 

Type Property

# min

The minimum representable integer in this type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var min: Int128 { get }
```

## Discussion

For unsigned integer types, this value is always `0`. For signed integer types, this value is `-(2 ** (bitWidth - 1))`, where `**` is exponentiation.

