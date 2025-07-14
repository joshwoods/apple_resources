

- Combine
- ImmediateScheduler
- ImmediateScheduler.SchedulerTimeType
- ImmediateScheduler.SchedulerTimeType.Stride
-  init(exactly:) 

Initializer

# init(exactly:)

Creates an immediate scheduler time interval from a binary integer type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init?(exactly source: T) where T : BinaryInteger
```

## Discussion

If `exactly` can’t convert to an `Int`, the resulting time interval is `nil`.

## See Also

### Creating Scheduler Time Strides

init(Int)

Creates an immediate scheduler time interval from the given time interval.

init(floatLiteral: Double)

Creates an immediate scheduler time interval from a floating-point seconds value.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(integerLiteral: Int)

Creates an immediate scheduler time interval from an integer seconds value.

