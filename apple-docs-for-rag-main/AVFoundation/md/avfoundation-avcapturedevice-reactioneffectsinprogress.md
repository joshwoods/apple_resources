

- AVFoundation
- AVCaptureDevice
-  reactionEffectsInProgress 

Instance Property

# reactionEffectsInProgress

An array of reaction effects that the device is currently performing, sorted by timestamp.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var reactionEffectsInProgress: [AVCaptureReactionEffectState] { get }
```

## Discussion

Key-value observe this property to determine when reaction effects begin and end. If your key-value observing callback provides old and new values, any in-progress reaction effects in the new array have a value of invalid for their endTime property value. Completed reaction effects are only in the old array, and have their endTime property value set to the presentation time of the first frame where the reaction effect was no longer present.

## See Also

### Performing Reaction Effects

class var reactionEffectsEnabled: Bool

A Boolean value that indicates whether the app supports performing reaction effects.

var canPerformReactionEffects: Bool

A Boolean value that indicates whether you can perform reaction effects on a capture device.

var availableReactionTypes: Set&lt;AVCaptureReactionType>

A set of reactions types that a device supports performing.

class var reactionEffectGesturesEnabled: Bool

A Boolean value that indicates whether gesture detection triggers reaction effects on the video stream.

func performEffect(for: AVCaptureReactionType)

Performs the specified reaction type on the video stream.

class AVCaptureReactionEffectState

An object that reports the state of a reaction effect performed on a capture device.

