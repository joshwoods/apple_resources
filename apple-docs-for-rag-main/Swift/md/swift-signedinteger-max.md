

- Swift
- SignedInteger
-  max 

Type Property

# max

The maximum representable integer in this type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var max: Self { get }
```

Available when `Self` conforms to `FixedWidthInteger`.

## Discussion

For signed integer types, this value is `(2 ** (bitWidth - 1)) - 1`, where `**` is exponentiation.

