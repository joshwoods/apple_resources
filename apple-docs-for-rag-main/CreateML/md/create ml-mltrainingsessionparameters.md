

- Create ML
-  MLTrainingSessionParameters 

Structure

# MLTrainingSessionParameters

The configuration settings for a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
struct MLTrainingSessionParameters
```

## Topics

### Creating a session’s parameters

init(sessionDirectory: URL?, reportInterval: Int, checkpointInterval: Int, iterations: Int)

Creates a set of parameters for a training session.

### Configuring the session’s parameters

let sessionDirectory: URL?

The location in the file system where the session stores its progress.

var reportInterval: Int

The number of iterations the session completes before it reports its progress.

var checkpointInterval: Int

The number of iterations the session completes before it saves a checkpoint.

var iterations: Int

The maximum number of iterations for the training session.

## Relationships

### Conforms To

- Sendable

## See Also

### Model Training Control

class MLJob

The representation of a model’s asynchronous training session you use to monitor the session’s progress or terminate its execution.

class MLTrainingSession

The current state of a model’s asynchronous training session.

struct MLCheckpoint

The state of a model’s asynchronous training session at a specific point in time during the feature extraction or training phase.

