

- Core Motion
-  CMStepQueryHandler 

Type Alias

# CMStepQueryHandler

A block that reports the number of steps for a query operation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
typealias CMStepQueryHandler = (Int, (any Error)?) -> Void
```

## Discussion

This block takes two parameters:

`numberOfSteps`  
The number of steps that occurred between the start and end times specified by the query.

`error`  
An error object indicating that there was a problem gathering the data or `nil` if the number of steps was determined correctly.

## See Also

### Getting Historical Step Counting Data

func queryStepCountStarting(from: Date, to: Date, to: OperationQueue, withHandler: CMStepQueryHandler)

Gathers and returns historical step count data for the specified time period.

Deprecated

