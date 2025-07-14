

- Swift
- Double
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

static var pi: Double

The mathematical constant pi (π), approximately equal to 3.14159.

static var infinity: Double

Positive infinity.

static var greatestFiniteMagnitude: Double

The greatest finite number representable by this type.

static var nan: Double

A quiet NaN (“not a number”).

static var signalingNaN: Double

A signaling NaN (“not a number”).

static var ulpOfOne: Double

The unit in the last place of 1.0.

static var leastNonzeroMagnitude: Double

The least positive number.

static var leastNormalMagnitude: Double

The least positive normal number.

