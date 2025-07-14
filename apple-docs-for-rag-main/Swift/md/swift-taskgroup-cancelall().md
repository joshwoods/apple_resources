

- Swift
- TaskGroup
-  cancelAll() 

Instance Method

# cancelAll()

Cancel all of the remaining tasks in the group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func cancelAll()
```

## Discussion

If you add a task to a group after canceling the group, that task is canceled immediately after being added to the group.

Immediately cancelled child tasks should therefore cooperatively check for and react to cancellation, e.g. by throwing an `CancellationError` at their earliest convenience, or otherwise handling the cancellation.

There are no restrictions on where you can call this method. Code inside a child task or even another task can cancel a group, however one should be very careful to not keep a reference to the group longer than the `with...TaskGroup(...) { ... }` method body is executing.

See Also

`Task.isCancelled`

See Also

`TaskGroup.isCancelled`

## See Also

### Canceling Tasks

var isCancelled: Bool

A Boolean value that indicates whether the group was canceled.

