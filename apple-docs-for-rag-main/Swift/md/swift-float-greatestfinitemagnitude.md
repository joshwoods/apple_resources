

- Swift
- Float
-  greatestFiniteMagnitude 

Type Property

# greatestFiniteMagnitude

The greatest finite number representable by this type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var greatestFiniteMagnitude: Float { get }
```

## Discussion

This value compares greater than or equal to all finite numbers, but less than `infinity`.

This value corresponds to type-specific C macros such as `FLT_MAX` and `DBL_MAX`. The naming of those macros is slightly misleading, because `infinity` is greater than this value.

## See Also

### Accessing Numeric Constants

static var pi: Float

The mathematical constant pi (π), approximately equal to 3.14159.

static var infinity: Float

Positive infinity.

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

static var zero: Self

The zero value.

