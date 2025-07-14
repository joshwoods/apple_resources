

- Create ML
-  MLCheckpoint 

Structure

# MLCheckpoint

The state of a model’s asynchronous training session at a specific point in time during the feature extraction or training phase.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
struct MLCheckpoint
```

## Topics

### Inspecting a checkpoint

var phase: MLPhase

The training session’s phase when it created the checkpoint.

var iteration: Int

The iteration number of a training session’s phase when it created the checkpoint.

var date: Date

The time when the training session created the checkpoint.

var url: URL

The location of the checkpoint in the file system.

### Assessing a checkpoint

var metrics: [MLProgress.Metric : Any]

Measurements of the model’s performance at the time the session saved the checkpoint.

enum Metric

Metrics you use to evaluate a model’s performance during a training session.

### Encoding and decoding a checkpoint

func encode(to: any Encoder) throws

Encodes the checkpoint into the encoder.

init(from: any Decoder) throws

Creates a new checkpoint by decoding from the decoder.

## Relationships

### Conforms To

- Decodable
- Encodable

## See Also

### Model Training Control

class MLJob

The representation of a model’s asynchronous training session you use to monitor the session’s progress or terminate its execution.

class MLTrainingSession

The current state of a model’s asynchronous training session.

struct MLTrainingSessionParameters

The configuration settings for a training session.

