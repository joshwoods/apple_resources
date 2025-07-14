

- Swift
- Task
-  checkCancellation() 

Type Method

# checkCancellation()

Throws an error if the task was canceled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func checkCancellation() throws
```

Available when `Success` is `Never` and `Failure` is `Never`.

## Discussion

The error is always an instance of `CancellationError`.

See Also

`isCancelled()`

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

func withTaskCancellationHandler&lt;T>(handler: () -> Void, operation: () async throws -> T) async rethrows -> TDeprecated

