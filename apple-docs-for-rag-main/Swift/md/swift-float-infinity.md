

- Swift
- Float
-  infinity 

Type Property

# infinity

Positive infinity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var infinity: Float { get }
```

## Discussion

Infinity compares greater than all finite numbers and equal to other infinite values.

```
let x = Double.greatestFiniteMagnitude
let y = x * 2
// y == Double.infinity
// y > x
```

## See Also

### Accessing Numeric Constants

static var pi: Float

The mathematical constant pi (π), approximately equal to 3.14159.

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

static var zero: Self

The zero value.

