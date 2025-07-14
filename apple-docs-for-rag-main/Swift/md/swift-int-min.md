

- Swift
- Int
-  min 

Type Property

# min

The minimum representable integer in this type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var min: Self { get }
```

Available when `Self` conforms to `FixedWidthInteger`.

## Discussion

For signed integer types, this value is `-(2 ** (bitWidth - 1))`, where `**` is exponentiation.

## See Also

### Accessing Numeric Constants

static var zero: Self

The zero value.

static var max: Self

The maximum representable integer in this type.

static var isSigned: Bool

A Boolean value indicating whether this type is a signed integer type.

