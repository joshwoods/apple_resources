

- Create ML
- MLTrainingSessionParameters
-  iterations 

Instance Property

# iterations

The maximum number of iterations for the training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var iterations: Int
```

## Discussion

Each iteration represents a full pass over the training data, also known as an epoch. Training may stop with fewer iterations if training converges. This limit also affects resumed training sessions. To extend training beyond the original limit, increase the limit before resuming.

## See Also

### Configuring the session’s parameters

let sessionDirectory: URL?

The location in the file system where the session stores its progress.

var reportInterval: Int

The number of iterations the session completes before it reports its progress.

var checkpointInterval: Int

The number of iterations the session completes before it saves a checkpoint.

