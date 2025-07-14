

- AVFoundation
- AVCaptureReactionEffectState
-  reactionType 

Instance Property

# reactionType

The type of reaction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var reactionType: AVCaptureReactionType { get }
```

## Discussion

There may be multiple reactions of the same type at a given time. Some may come from calls to performEffect(for:) and others from gesture detection.

## See Also

### Configuring the effect state

struct AVCaptureReactionType

Constants that indicate the type of reaction that an effect can perform.

var startTime: CMTime

The presentation time of the first frame where the system renders the effect.

var endTime: CMTime

The presentation time of the first frame following the end of a reaction effect.

