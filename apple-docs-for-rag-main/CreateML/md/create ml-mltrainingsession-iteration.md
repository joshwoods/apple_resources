

- Create ML
- MLTrainingSession
-  iteration 

Instance Property

# iteration

The iteration number of a training session’s phase.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
final var iteration: Int { get }
```

## See Also

### Checking a training session’s progress

var phase: MLPhase

The training session’s current state.

enum MLPhase

The possible states of a training session.

var checkpoints: [MLCheckpoint]

An array of checkpoints the training session has created so far.

