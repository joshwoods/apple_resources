

- Swift
- Float
-  signalingNaN 

Type Property

# signalingNaN

A signaling NaN (“not a number”).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var signalingNaN: Float { get }
```

## Discussion

The default IEEE 754 behavior of operations involving a signaling NaN is to raise the Invalid flag in the floating-point environment and return a quiet NaN.

Operations on types conforming to the `FloatingPoint` protocol should support this behavior, but they might also support other options. For example, it would be reasonable to implement alternative operations in which operating on a signaling NaN triggers a runtime error or results in a diagnostic for debugging purposes. Types that implement alternative behaviors for a signaling NaN must document the departure.

Other than these signaling operations, a signaling NaN behaves in the same manner as a quiet NaN.

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

static var ulpOfOne: Float

The unit in the last place of 1.0.

static var leastNormalMagnitude: Float

The least positive normal number.

static var leastNonzeroMagnitude: Float

The least positive number.

static var zero: Self

The zero value.

