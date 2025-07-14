

- Swift
- Float
-  ulpOfOne 

Type Property

# ulpOfOne

The unit in the last place of 1.0.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var ulpOfOne: Float { get }
```

## Discussion

The positive difference between 1.0 and the next greater representable number. The `ulpOfOne` constant corresponds to the C macros `FLT_EPSILON`, `DBL_EPSILON`, and others with a similar purpose.

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

static var leastNormalMagnitude: Float

The least positive normal number.

static var leastNonzeroMagnitude: Float

The least positive number.

static var zero: Self

The zero value.

