

- AVFoundation
- AVCaptureDevice
-  reactionEffectsEnabled 

Type Property

# reactionEffectsEnabled

A Boolean value that indicates whether the app supports performing reaction effects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class var reactionEffectsEnabled: Bool { get }
```

## Discussion

The system only renders reaction effects when the device’s active format supports the feature, which you determine by querying the value of its reactionEffectsSupported property.

In macOS, the system enables reaction effects for all apps by default. In iOS, it enables them by default only for video conferencing apps (apps that enable the Voice over IP option in their UIBackgroundModes configuration). Apps that don’t use this background mode may opt in to this feature by adding the following key to the `Info.plist` file.

```
NSCameraReactionEffectsEnabled

```

## See Also

### Performing Reaction Effects

var canPerformReactionEffects: Bool

A Boolean value that indicates whether you can perform reaction effects on a capture device.

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

