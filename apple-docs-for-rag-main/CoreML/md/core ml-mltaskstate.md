

- Core ML
-  MLTaskState 

Enumeration

# MLTaskState

The state of a machine learning task.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
enum MLTaskState
```

## Topics

### Transient States

case running

The state of a machine learning task that’s executing.

case suspended

The state of a machine learning task that’s paused.

case cancelling

The state of a machine learning task that’s in mid-termination, before it could finish successfully.

### Final States

case completed

The state of a machine learning task that has finished successfully.

case failed

The state of a machine learning task that has terminated due to an error.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking the State of a Task

var state: MLTaskState

The current state of the machine learning task.

var error: (any Error)?

The underlying error if the task is in a failed state.

