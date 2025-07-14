

- ClassKit
- CLSProgressReportingCapability
- CLSProgressReportingCapability.Kind
-  CLSProgressReportingCapability.Kind.percent 

Case

# CLSProgressReportingCapability.Kind.percent

The percentage of the total task that has been completed.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
case percent
```

## Discussion

Add this capability to indicate that a context reports a task’s percentage completion on a periodic basis by setting the associated activity’s progress property, or by calling the activity’s addProgressRange(fromStart:toEnd:) method.

## See Also

### Reporting Capabilities

case duration

Time spent performing the task.

case binary

A binary outcome for the task, like true or false.

case quantity

A discrete value.

case score

A score.

