

- Foundation
- URL Loading System
- URLSessionTask
-  URL session task priority 

API Collection

# URL session task priority

Constants for providing task priority hints to a host, used with the priority property.

## Topics

### Priority constants

class let defaultPriority: Float

The default URL session task priority, used implicitly for any task you have not prioritized.

class let lowPriority: Float

A low URL session task priority, with a floating point value above the minimum of `0` and below the default value.

class let highPriority: Float

A high URL session task priority, with a floating point value above the default value and below the maximum of `1.0`.

## See Also

### Controlling the task state

func cancel()

Cancels the task.

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

