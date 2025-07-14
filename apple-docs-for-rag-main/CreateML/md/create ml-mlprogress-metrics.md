

- Create ML
- MLProgress
-  metrics 

Instance Property

# metrics

Measurements of the model’s performance during the training or evaluation phases of a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var metrics: [MLProgress.Metric : Any]
```

## See Also

### Inspecting a session’s progress

var elapsedTime: TimeInterval

The time, in seconds, since the training session started.

var phase: MLPhase

The current phase of the training session.

var itemCount: Int

The current number of files processed during a feature extraction phase, or the completed iterations during a training phase.

var totalItemCount: Int?

The total number of files during a feature extraction phase, or total iterations during a training phase.

enum Metric

Metrics you use to evaluate a model’s performance during a training session.

