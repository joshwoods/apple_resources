

- Foundation
- URLSessionTask
-  cancel() 

Instance Method

# cancel()

Cancels the task.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancel()
```

## Discussion

This method returns immediately, marking the task as being canceled. Once a task is marked as being canceled, urlSession(_:task:didCompleteWithError:) will be sent to the task delegate, passing an error in the domain NSURLErrorDomain with the code NSURLErrorCancelled. A task may, under some circumstances, send messages to its delegate before the cancelation is acknowledged.

This method may be called on a task that is suspended.

## See Also

### Related Documentation

func cancel(byProducingResumeData: (Data?) -> Void)

Cancels a download and calls a callback with resume data for later use.

### Controlling the task state

func resume()

Resumes the task, if it is suspended.

func suspend()

Temporarily suspends a task.

var state: URLSessionTask.State

The current state of the task—active, suspended, in the process of being canceled, or completed.

enum State

Constants for determining the current state of a task.

var priority: Float

The relative priority at which you’d like a host to handle the task, specified as a floating point value between `0.0` (lowest priority) and `1.0` (highest priority).

URL session task priority

Constants for providing task priority hints to a host, used with the priority property.

