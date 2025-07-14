

- AVFoundation
- AVCaptureDevice
-  availableReactionTypes 

Instance Property

# availableReactionTypes

A set of reactions types that a device supports performing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var availableReactionTypes: Set { get }
```

## Discussion

The list may differ between devices, and may change for a specific device when it’s active format changes.

This property is key-value observable.

## See Also

### Performing Reaction Effects

class var reactionEffectsEnabled: Bool

A Boolean value that indicates whether the app supports performing reaction effects.

var canPerformReactionEffects: Bool

A Boolean value that indicates whether you can perform reaction effects on a capture device.

class var reactionEffectGesturesEnabled: Bool

A Boolean value that indicates whether gesture detection triggers reaction effects on the video stream.

func performEffect(for: AVCaptureReactionType)

Performs the specified reaction type on the video stream.

var reactionEffectsInProgress: [AVCaptureReactionEffectState]

An array of reaction effects that the device is currently performing, sorted by timestamp.

class AVCaptureReactionEffectState

An object that reports the state of a reaction effect performed on a capture device.

