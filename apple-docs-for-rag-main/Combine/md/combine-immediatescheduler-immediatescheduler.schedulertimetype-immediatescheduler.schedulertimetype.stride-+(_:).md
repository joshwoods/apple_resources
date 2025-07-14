

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
- ImmediateScheduler.SchedulerTimeType.Stride
-  +(\_:) 

Operator

# +(\_:)

Returns the given number unchanged.

CombineSwiftiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func + (x: Self) -> Self
```

## Return Value

The given argument without any changes.

## Discussion

You can use the unary plus operator (`+`) to provide symmetry in your code for positive numbers when also using the unary minus operator.

```
let x = -21
let y = +21
// x == -21
// y == 21
```

## See Also

### Performing Mathematical Operations

func negate()

Replaces this value with its additive inverse.

static func * (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Multiplies two values and produces their product.

static func *= (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Multiplies two values and stores the result in the left-hand-side variable.

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

