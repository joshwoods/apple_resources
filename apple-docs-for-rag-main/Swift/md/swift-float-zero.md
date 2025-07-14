

- Swift
- Float
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

static var pi: Float

The mathematical constant pi (π), approximately equal to 3.14159.

static var infinity: Float

Positive infinity.

static var greatestFiniteMagnitude: Float

The greatest finite number representable by this type.

static var nan: Float

A quiet NaN (“not a number”).

static var signalingNaN: Float

A signaling NaN (“not a number”).

static var ulpOfOne: Float

The unit in the last place of 1.0.

static var leastNormalMagnitude: Float

The least positive normal number.

static var leastNonzeroMagnitude: Float

The least positive number.

