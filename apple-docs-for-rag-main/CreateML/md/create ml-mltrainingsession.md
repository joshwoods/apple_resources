

- Create ML
-  MLTrainingSession 

Class

# MLTrainingSession

The current state of a model’s asynchronous training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
final class MLTrainingSession
```

## Topics

### Checking a training session’s progress

var phase: MLPhase

The training session’s current state.

enum MLPhase

The possible states of a training session.

var iteration: Int

The iteration number of a training session’s phase.

var checkpoints: [MLCheckpoint]

An array of checkpoints the training session has created so far.

### Removing checkpoints

func removeCheckpoints((MLCheckpoint) -> Bool) throws

Removes the checkpoints that satisfy your closure from the training session.

### Reusing features from a previous session

func reuseExtractedFeatures(from: MLTrainingSession&lt;Task>) throws

Uses the features another session has already extracted from its dataset.

### Inspecting a session

var date: Date

The time when you created this training session.

let parameters: MLTrainingSessionParameters

The parameters you used to create the training session.

## Relationships

### Conforms To

- Sendable

## See Also

### Model Training Control

class MLJob

The representation of a model’s asynchronous training session you use to monitor the session’s progress or terminate its execution.

struct MLTrainingSessionParameters

The configuration settings for a training session.

struct MLCheckpoint

The state of a model’s asynchronous training session at a specific point in time during the feature extraction or training phase.

