

- MetricKit
- MXError
- MXError.Code
-  MXError.Code.launchTaskInternalFailure 

Case

# MXError.Code.launchTaskInternalFailure

Internal failures happened inside the framework.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
case launchTaskInternalFailure
```

## See Also

### Launch errors

case launchTaskDuplicated

A task with the same ID has already been started.

case launchTaskInvalidID

The task ID is a `null` value or exceeds the maximum 128 character length.

case launchTaskMaxCount

Exceeded the maximum number of tasks.

case launchTaskPastDeadline

The start call was made too late.

case launchTaskUnknown

The task hasn’t been started or has already been finished.

