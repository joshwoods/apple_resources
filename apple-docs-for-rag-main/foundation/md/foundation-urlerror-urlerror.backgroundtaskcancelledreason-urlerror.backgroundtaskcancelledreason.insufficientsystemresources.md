

- Foundation
- URLError
- URLError.BackgroundTaskCancelledReason
-  URLError.BackgroundTaskCancelledReason.insufficientSystemResources 

Case

# URLError.BackgroundTaskCancelledReason.insufficientSystemResources

A reason that indicates the system canceled the background task because it lacks sufficient resources to perform the task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case insufficientSystemResources
```

## Discussion

This error results from factors including (but not limited to) battery capacity, thermal condition, network connectivity, and cellular data plan.

## See Also

### Cancellation reasons

case backgroundUpdatesDisabled

A reason that indicates the system canceled the background task because background tasks are disabled.

case userForceQuitApplication

A reason that indicates the system canceled the background task because the user force-quit the application.

