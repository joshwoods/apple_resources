

- Foundation
- URLSessionTask
-  state 

Instance Property

# state

The current state of the task—active, suspended, in the process of being canceled, or completed.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var state: URLSessionTask.State { get }
```

## See Also

### Controlling the task state

func cancel()

Cancels the task.

func resume()

Resumes the task, if it is suspended.

func suspend()

Temporarily suspends a task.

enum State

Constants for determining the current state of a task.

var priority: Float

The relative priority at which you’d like a host to handle the task, specified as a floating point value between `0.0` (lowest priority) and `1.0` (highest priority).

URL session task priority

Constants for providing task priority hints to a host, used with the priority property.

