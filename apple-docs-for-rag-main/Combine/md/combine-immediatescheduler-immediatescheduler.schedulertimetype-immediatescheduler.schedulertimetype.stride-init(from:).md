

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
- ImmediateScheduler.SchedulerTimeType.Stride
-  init(from:) 

Initializer

# init(from:)

Creates a new instance by decoding from the given decoder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

## See Also

### Creating Scheduler Time Strides

init(Int)

Creates an immediate scheduler time interval from the given time interval.

init?&lt;T>(exactly: T)

Creates an immediate scheduler time interval from a binary integer type.

init(floatLiteral: Double)

Creates an immediate scheduler time interval from a floating-point seconds value.

init(integerLiteral: Int)

Creates an immediate scheduler time interval from an integer seconds value.

