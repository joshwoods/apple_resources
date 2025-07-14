

- Create ML
- MLTrainingSessionParameters
-  sessionDirectory 

Instance Property

# sessionDirectory

The location in the file system where the session stores its progress.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
let sessionDirectory: URL?
```

## See Also

### Configuring the session’s parameters

var reportInterval: Int

The number of iterations the session completes before it reports its progress.

var checkpointInterval: Int

The number of iterations the session completes before it saves a checkpoint.

var iterations: Int

The maximum number of iterations for the training session.

