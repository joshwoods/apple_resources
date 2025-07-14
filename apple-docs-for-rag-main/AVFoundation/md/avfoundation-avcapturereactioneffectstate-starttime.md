

- AVFoundation
- AVCaptureReactionEffectState
-  startTime 

Instance Property

# startTime

The presentation time of the first frame where the system renders the effect.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var startTime: CMTime { get }
```

## See Also

### Configuring the effect state

var reactionType: AVCaptureReactionType

The type of reaction.

struct AVCaptureReactionType

Constants that indicate the type of reaction that an effect can perform.

var endTime: CMTime

The presentation time of the first frame following the end of a reaction effect.

