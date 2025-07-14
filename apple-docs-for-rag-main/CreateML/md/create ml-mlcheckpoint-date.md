

- Create ML
- MLCheckpoint
-  date 

Instance Property

# date

The time when the training session created the checkpoint.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var date: Date
```

## See Also

### Inspecting a checkpoint

var phase: MLPhase

The training session’s phase when it created the checkpoint.

var iteration: Int

The iteration number of a training session’s phase when it created the checkpoint.

var url: URL

The location of the checkpoint in the file system.

