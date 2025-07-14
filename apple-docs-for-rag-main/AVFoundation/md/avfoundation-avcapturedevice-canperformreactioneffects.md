

- AVFoundation
- AVCaptureDevice
-  canPerformReactionEffects 

Instance Property

# canPerformReactionEffects

A Boolean value that indicates whether you can perform reaction effects on a capture device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var canPerformReactionEffects: Bool { get }
```

## Discussion

This value is true when a device’s reactionEffectsEnabled and its active format’s reactionEffectsSupported property values are true.

## See Also

### Performing Reaction Effects

class var reactionEffectsEnabled: Bool

A Boolean value that indicates whether the app supports performing reaction effects.

var availableReactionTypes: Set&lt;AVCaptureReactionType>

A set of reactions types that a device supports performing.

class var reactionEffectGesturesEnabled: Bool

A Boolean value that indicates whether gesture detection triggers reaction effects on the video stream.

func performEffect(for: AVCaptureReactionType)

Performs the specified reaction type on the video stream.

var reactionEffectsInProgress: [AVCaptureReactionEffectState]

An array of reaction effects that the device is currently performing, sorted by timestamp.

class AVCaptureReactionEffectState

An object that reports the state of a reaction effect performed on a capture device.

