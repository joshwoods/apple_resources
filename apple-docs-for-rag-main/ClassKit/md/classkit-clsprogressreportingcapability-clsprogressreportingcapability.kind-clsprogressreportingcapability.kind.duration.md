

- ClassKit
- CLSProgressReportingCapability
- CLSProgressReportingCapability.Kind
-  CLSProgressReportingCapability.Kind.duration 

Case

# CLSProgressReportingCapability.Kind.duration

Time spent performing the task.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
case duration
```

## Discussion

The framework automatically measures the time that a student spends working on a task, so all contexts have a CLSProgressReportingCapability.Kind.duration capability by default. You can replace the default one with a new one if you want to customize the details string.

## See Also

### Reporting Capabilities

case percent

The percentage of the total task that has been completed.

case binary

A binary outcome for the task, like true or false.

case quantity

A discrete value.

case score

A score.

