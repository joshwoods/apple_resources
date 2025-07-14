

- AVFoundation
- AVCaptureReactionEffectState
-  endTime 

Instance Property

# endTime

The presentation time of the first frame following the end of a reaction effect.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var endTime: CMTime { get }
```

## Discussion

The value is invalid while the effect is in progress, but changes to a valid time when the reaction effect completes and the system removes it from the list of reactionEffectsInProgress.

## See Also

### Configuring the effect state

var reactionType: AVCaptureReactionType

The type of reaction.

struct AVCaptureReactionType

Constants that indicate the type of reaction that an effect can perform.

var startTime: CMTime

The presentation time of the first frame where the system renders the effect.

