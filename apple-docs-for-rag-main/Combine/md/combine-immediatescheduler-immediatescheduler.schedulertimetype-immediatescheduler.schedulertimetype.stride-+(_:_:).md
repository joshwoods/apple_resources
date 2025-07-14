

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
- ImmediateScheduler.SchedulerTimeType.Stride
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Adds two values and produces their sum.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func + (lhs: ImmediateScheduler.SchedulerTimeType.Stride, rhs: ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride
```

## Parameters 

`lhs`  

The first value to add.

`rhs`  

The second value to add.

## Discussion

The addition operator (`+`) calculates the sum of its two arguments. For example:

```
1 + 2                   // 3
-10 + 15                // 5
-15 + -5                // -20
21.5 + 3.25             // 24.75
```

You cannot use `+` with arguments of different types. To add values of different types, convert one of the values to the other value’s type.

```
let x: Int8 = 21
let y: Int = 1000000
Int(x) + y              // 1000021
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

static func += (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Adds two values and stores the result in the left-hand-side variable.

static func - (Self) -> Self

Returns the additive inverse of the specified value.

static func - (ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride) -> ImmediateScheduler.SchedulerTimeType.Stride

Subtracts one value from another and produces their difference.

static func -= (inout ImmediateScheduler.SchedulerTimeType.Stride, ImmediateScheduler.SchedulerTimeType.Stride)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

