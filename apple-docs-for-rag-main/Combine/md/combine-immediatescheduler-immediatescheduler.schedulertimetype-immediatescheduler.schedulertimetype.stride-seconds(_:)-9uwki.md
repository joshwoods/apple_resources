

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
- ImmediateScheduler.SchedulerTimeType.Stride
-  seconds(\_:) 

Type Method

# seconds(\_:)

Converts the specified number of seconds into an instance of this scheduler time type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func seconds(_ s: Int) -> ImmediateScheduler.SchedulerTimeType.Stride
```

## See Also

### Creating Scheduler Time Strides from Seconds

static func microseconds(Int) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of microseconds into an instance of this scheduler time type.

static func milliseconds(Int) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of milliseconds into an instance of this scheduler time type.

static func nanoseconds(Int) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of nanoseconds into an instance of this scheduler time type.

static func seconds(Double) -> ImmediateScheduler.SchedulerTimeType.Stride

Converts the specified number of seconds, as a floating-point value, into an instance of this scheduler time type.

