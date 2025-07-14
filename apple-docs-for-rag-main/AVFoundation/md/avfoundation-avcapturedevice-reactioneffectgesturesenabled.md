

- AVFoundation
- AVCaptureDevice
-  reactionEffectGesturesEnabled 

Type Property

# reactionEffectGesturesEnabled

A Boolean value that indicates whether gesture detection triggers reaction effects on the video stream.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class var reactionEffectGesturesEnabled: Bool { get }
```

## Discussion

This property reflects the enabled state of Gestures in Control Center.

Gesture detection runs only when the device’s active format supports reaction effects, which you determine by querying the value of the format’s reactionEffectsSupported property.

This property is key-value observable.

Note

Your app can call performEffect(for:)independently the value of this property. The system intermixes reaction effects from either source.

## See Also

### Performing Reaction Effects

class var reactionEffectsEnabled: Bool

A Boolean value that indicates whether the app supports performing reaction effects.

var canPerformReactionEffects: Bool

A Boolean value that indicates whether you can perform reaction effects on a capture device.

var availableReactionTypes: Set&lt;AVCaptureReactionType>

A set of reactions types that a device supports performing.

func performEffect(for: AVCaptureReactionType)

Performs the specified reaction type on the video stream.

var reactionEffectsInProgress: [AVCaptureReactionEffectState]

An array of reaction effects that the device is currently performing, sorted by timestamp.

class AVCaptureReactionEffectState

An object that reports the state of a reaction effect performed on a capture device.

