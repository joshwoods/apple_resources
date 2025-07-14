

- Foundation
-  NSURLErrorCancelledReasonInsufficientSystemResources 

Global Variable

# NSURLErrorCancelledReasonInsufficientSystemResources

A reason that indicates the system canceled the background task because it lacks sufficient resources to perform the task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var NSURLErrorCancelledReasonInsufficientSystemResources: Int { get }
```

## Discussion

This error results from factors including (but not limited to) battery capacity, thermal condition, network connectivity, and cellular data plan.

## See Also

### Cancellation reasons

var NSURLErrorCancelledReasonBackgroundUpdatesDisabled: Int

A reason that indicates the system canceled the background task because background tasks are disabled.

var NSURLErrorCancelledReasonUserForceQuitApplication: Int

A reason that indicates the system canceled the background task because the user force-quit the application.

