

- MetricKit
- MXError
- MXError.Code
-  MXError.Code.launchTaskPastDeadline 

Case

# MXError.Code.launchTaskPastDeadline

The start call was made too late.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
case launchTaskPastDeadline
```

## See Also

### Launch errors

case launchTaskDuplicated

A task with the same ID has already been started.

case launchTaskInternalFailure

Internal failures happened inside the framework.

case launchTaskInvalidID

The task ID is a `null` value or exceeds the maximum 128 character length.

case launchTaskMaxCount

Exceeded the maximum number of tasks.

case launchTaskUnknown

The task hasn’t been started or has already been finished.

