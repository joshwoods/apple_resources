

- Swift
- Task
-  isCancelled 

Type Property

# isCancelled

A Boolean value that indicates whether the task should stop executing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var isCancelled: Bool { get }
```

Available when `Success` is `Never` and `Failure` is `Never`.

## Discussion

After the value of this property becomes `true`, it remains `true` indefinitely. There is no way to uncancel a task.

See Also

`checkCancellation()`

## See Also

### Canceling Tasks

struct CancellationError

An error that indicates a task was canceled.

func cancel()

Cancels this task.

var isCancelled: Bool

A Boolean value that indicates whether the task should stop executing.

static func checkCancellation() throws

Throws an error if the task was canceled.

func withTaskCancellationHandler&lt;T>(handler: () -> Void, operation: () async throws -> T) async rethrows -> TDeprecated

