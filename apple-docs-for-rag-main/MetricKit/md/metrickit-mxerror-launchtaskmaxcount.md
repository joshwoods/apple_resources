

- MetricKit
- MXError
-  launchTaskMaxCount 

Type Property

# launchTaskMaxCount

Exceeded the maximum number of tasks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
static var launchTaskMaxCount: MXError.Code { get }
```

## See Also

### Getting the launch error properties

static var launchTaskDuplicated: MXError.Code

A task with the same ID has already been started.

static var launchTaskInternalFailure: MXError.Code

Internal failures happened inside the framework.

static var launchTaskInvalidID: MXError.Code

The task ID is a `null` value or exceeds the maximum 128 character length.

static var launchTaskPastDeadline: MXError.Code

The start call was made too late.

static var launchTaskUnknown: MXError.Code

The task hasn’t been started or has already been finished.

enum Code

Error codes for error values from app metrics.

let MXErrorDomain: String

Error domain for error values from app metrics.

