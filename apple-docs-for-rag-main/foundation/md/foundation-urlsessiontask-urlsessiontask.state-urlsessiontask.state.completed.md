

- Foundation
- URLSessionTask
- URLSessionTask.State
-  URLSessionTask.State.completed 

Case

# URLSessionTask.State.completed

The task has completed (without being canceled), and the task’s delegate receives no further callbacks.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case completed
```

## Discussion

If the task completed successfully, the task’s error property is `nil`. Otherwise, it provides an error object that tells what went wrong. A task in this state is not subject to timeouts.

## See Also

### Task states

case running

The task is currently being serviced by the session.

case suspended

The task was suspended by the app.

case canceling

The task has received a `cancel` message.

