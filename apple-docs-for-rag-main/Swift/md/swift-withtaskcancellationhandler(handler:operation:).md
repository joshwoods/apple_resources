

- Swift
-  withTaskCancellationHandler(handler:operation:) 

Function

# withTaskCancellationHandler(handler:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func withTaskCancellationHandler(
    handler: () -> Void,
    operation: () async throws -> T
) async rethrows -> T
```

## See Also

### Canceling Tasks

struct CancellationError

An error that indicates a task was canceled.

func cancel()

Cancels this task.

var isCancelled: Bool

A Boolean value that indicates whether the task should stop executing.

static var isCancelled: Bool

A Boolean value that indicates whether the task should stop executing.

static func checkCancellation() throws

Throws an error if the task was canceled.

