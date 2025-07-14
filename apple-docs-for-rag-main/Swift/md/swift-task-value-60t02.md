

- Swift
- Task
-  value 

Instance Property

# value

The result from a throwing task, after it completes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var value: Success { get async throws }
```

Available when `Success` conforms to `Sendable` and `Failure` conforms to `Error`.

## Return Value

The task’s result.

## Discussion

If the task hasn’t completed, accessing this property waits for it to complete and its priority increases to that of the current task. Note that this might not be as effective as creating the task with the correct priority, depending on the executor’s scheduling details.

If the task throws an error, this property propagates that error. Tasks that respond to cancellation by throwing `CancellationError` have that error propagated here upon cancellation.

## See Also

### Accessing Results

var value: Success

The result from a nonthrowing task, after it completes.

var result: Result&lt;Success, Failure>

The result or error from a throwing task, after it completes.

