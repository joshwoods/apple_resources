

- Foundation
- URLSessionTask
-  suspend() 

Instance Method

# suspend()

Temporarily suspends a task.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func suspend()
```

## Discussion

A task, while suspended, produces no network traffic and isn’t subject to timeouts. Call resume() to resume data transfer.

## See Also

### Related Documentation

func cancel(byProducingResumeData: (Data?) -> Void)

Cancels a download and calls a callback with resume data for later use.

### Controlling the task state

func cancel()

Cancels the task.

func resume()

Resumes the task, if it is suspended.

var state: URLSessionTask.State

The current state of the task—active, suspended, in the process of being canceled, or completed.

enum State

Constants for determining the current state of a task.

var priority: Float

The relative priority at which you’d like a host to handle the task, specified as a floating point value between `0.0` (lowest priority) and `1.0` (highest priority).

URL session task priority

Constants for providing task priority hints to a host, used with the priority property.

