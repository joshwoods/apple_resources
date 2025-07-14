

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
- ImmediateScheduler.SchedulerTimeType.Stride
-  -(\_:) 

Operator

# -(\_:)

Returns the additive inverse of the specified value.

CombineSwiftiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func - (operand: Self) -> Self
```

## Return Value

The additive inverse of this value.

## Discussion

The negation operator (prefix `-`) returns the additive inverse of its argument.

```
let x = 21
let y = -x
// y == -21
```

The resulting value must be representable in the same type as the argument. In particular, negating a signed, fixed-width integer type’s minimum results in a value that cannot be represented.

```
let z = -Int8.min
// Overflow error
```

## See Also

### Performing Mathematical Operations

func negate()

Replaces this value with its additive inverse.

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

static func - (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Subtracts one value from another and produces their difference.

static func -= (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

