

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
- ImmediateScheduler.SchedulerTimeType.Stride
-  negate() 

Instance Method

# negate()

Replaces this value with its additive inverse.

CombineSwiftiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func negate()
```

## Discussion

The following example uses the `negate()` method to negate the value of an integer `x`:

```
var x = 21
x.negate()
// x == -21
```

The resulting value must be representable within the value’s type. In particular, negating a signed, fixed-width integer type’s minimum results in a value that cannot be represented.

```
var y = Int8.min
y.negate()
// Overflow error
```

## See Also

### Performing Mathematical Operations

static func * (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Multiplies two values and produces their product.

static func *= (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Multiplies two values and stores the result in the left-hand-side variable.

static func + (Self) -> Self

Returns the given number unchanged.

static func + (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Adds two values and produces their sum.

static func += (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Adds two values and stores the result in the left-hand-side variable.

static func - (Self) -> Self

Returns the additive inverse of the specified value.

static func - (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Subtracts one value from another and produces their difference.

static func -= (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

