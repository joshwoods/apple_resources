

- Foundation
- URLSessionTask
-  delegate 

Instance Property

# delegate

A delegate specific to the task.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var delegate: (any URLSessionTaskDelegate)? { get set }
```

## Discussion

This task-specific delegate receives messages from the task before the session’s delegate receives them. This is similar to the behavior of the `delegate` parameter used by the asychronous methods in URLSession like bytes(for:delegate:) and data(for:delegate:).

## See Also

### Using a task-specific delegate

protocol URLSessionTaskDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events.

