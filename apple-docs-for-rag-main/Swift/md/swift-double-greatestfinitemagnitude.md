

- Swift
- Double
-  greatestFiniteMagnitude 

Type Property

# greatestFiniteMagnitude

The greatest finite number representable by this type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var greatestFiniteMagnitude: Double { get }
```

## Discussion

This value compares greater than or equal to all finite numbers, but less than `infinity`.

This value corresponds to type-specific C macros such as `FLT_MAX` and `DBL_MAX`. The naming of those macros is slightly misleading, because `infinity` is greater than this value.

## See Also

### Accessing Numeric Constants

static var pi: Double

The mathematical constant pi (π), approximately equal to 3.14159.

static var infinity: Double

Positive infinity.

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

static var zero: Self

The zero value.

