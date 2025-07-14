

- Swift
- Int
-  zero 

Type Property

# zero

The zero value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var zero: Self { get }
```

Available when `Self` conforms to `ExpressibleByIntegerLiteral`.

## Discussion

Zero is the identity element for addition. For any value, `x + .zero == x` and `.zero + x == x`.

## See Also

### Accessing Numeric Constants

static var min: Self

The minimum representable integer in this type.

static var max: Self

The maximum representable integer in this type.

static var isSigned: Bool

A Boolean value indicating whether this type is a signed integer type.

