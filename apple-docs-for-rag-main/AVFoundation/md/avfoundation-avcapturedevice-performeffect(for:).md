

- AVFoundation
- AVCaptureDevice
-  performEffect(for:) 

Instance Method

# performEffect(for:)

Performs the specified reaction type on the video stream.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
func performEffect(for reactionType: AVCaptureReactionType)
```

## Parameters 

`reactionType`  

A reaction type to perform. Specifying a type that doesn’t exists within the set of availableReactionTypes for the device results in an exception.

## Discussion

The entries in the reactionEffectsInProgress property may not reflect one-to-one with calls to this method. Depending on reaction style or resource limits, the system may coalesce overlapping reactions of the same type by extending an existing reaction rather than overlaying a new one.

Note

Calling this method has no effect when the value of canPerformReactionEffects is false. In this case, VoIP apps should transmit and display reactions outside of the video feed.

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

var reactionEffectsInProgress: [AVCaptureReactionEffectState]

An array of reaction effects that the device is currently performing, sorted by timestamp.

class AVCaptureReactionEffectState

An object that reports the state of a reaction effect performed on a capture device.

