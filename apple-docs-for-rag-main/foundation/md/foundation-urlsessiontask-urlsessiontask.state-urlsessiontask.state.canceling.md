

- Foundation
- URLSessionTask
- URLSessionTask.State
-  URLSessionTask.State.canceling 

Case

# URLSessionTask.State.canceling

The task has received a `cancel` message.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case canceling
```

## Discussion

The delegate may or may not have received a urlSession(_:task:didCompleteWithError:) message yet. A task in this state is not subject to timeouts.

## See Also

### Task states

case running

The task is currently being serviced by the session.

case suspended

The task was suspended by the app.

case completed

The task has completed (without being canceled), and the task’s delegate receives no further callbacks.

