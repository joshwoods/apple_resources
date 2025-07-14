

- Core ML
-  MLTask 

Class

# MLTask

An abstract base class for machine learning tasks.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class MLTask
```

## Overview

You don’t create use this class directly. Instead, use a class that inherits from this one, such as MLUpdateTask.

## Topics

### Identifying a Task

var taskIdentifier: String

A unique name of the task to distinguish it from all other tasks at runtime.

### Starting and Stopping a Task

func resume()

Begins or resumes a machine learning task.

func cancel()

Cancels a machine learning task before it completes.

### Checking the State of a Task

var state: MLTaskState

The current state of the machine learning task.

enum MLTaskState

The state of a machine learning task.

var error: (any Error)?

The underlying error if the task is in a failed state.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MLUpdateTask

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### On-Device Model Updates

Personalizing a Model with On-Device Updates

Modify an updatable Core ML model by running an update task with labeled data.

class MLUpdateTask

A task that updates a model with additional training data.

