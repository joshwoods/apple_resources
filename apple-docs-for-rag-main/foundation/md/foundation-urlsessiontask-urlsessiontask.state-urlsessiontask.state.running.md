

- Foundation
- URLSessionTask
- URLSessionTask.State
-  URLSessionTask.State.running 

Case

# URLSessionTask.State.running

The task is currently being serviced by the session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case running
```

## Discussion

A task in this state is subject to the request and resource timeouts specified in the session configuration object.

## See Also

### Task states

case suspended

The task was suspended by the app.

case canceling

The task has received a `cancel` message.

case completed

The task has completed (without being canceled), and the task’s delegate receives no further callbacks.

