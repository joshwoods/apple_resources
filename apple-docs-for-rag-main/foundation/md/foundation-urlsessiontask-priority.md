

- Foundation
- URLSessionTask
-  priority 

Instance Property

# priority

The relative priority at which you’d like a host to handle the task, specified as a floating point value between `0.0` (lowest priority) and `1.0` (highest priority).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var priority: Float { get set }
```

## Discussion

To provide hints to a host on how to prioritize URL session tasks from your app, specify a priority for each task. Specifying a priority provides only a hint and does not guarantee performance. If you don’t specify a priority, a URL session task has a priority of defaultPriority, with a value of `0.5`.

There are three named priorities you can employ, described in URL session task priority.

You can specify or change a task’s priority at any time, but not all networking protocols respond to changes after a task has started. There is no API to let you determine the effective priority for a task from a host’s perspective.

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

URL session task priority

Constants for providing task priority hints to a host, used with the priority property.

