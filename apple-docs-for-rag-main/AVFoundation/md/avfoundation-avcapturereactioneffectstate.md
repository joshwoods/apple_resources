

- AVFoundation
-  AVCaptureReactionEffectState 

Class

# AVCaptureReactionEffectState

An object that reports the state of a reaction effect performed on a capture device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class AVCaptureReactionEffectState
```

## Overview

Obtain an instance of this class by querying a capture device’s reactionEffectsInProgress property. The system adds new entries to this array when you call performEffect(for:) or by gesture detection in the capture stream when the value of reactionEffectGesturesEnabled is true.

The system renders the effect before providing frames to your app, and these status objects let you know when it performs the effect.

## Topics

### Configuring the effect state

var reactionType: AVCaptureReactionType

The type of reaction.

struct AVCaptureReactionType

Constants that indicate the type of reaction that an effect can perform.

var startTime: CMTime

The presentation time of the first frame where the system renders the effect.

var endTime: CMTime

The presentation time of the first frame following the end of a reaction effect.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

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

var reactionEffectsInProgress: [AVCaptureReactionEffectState]

An array of reaction effects that the device is currently performing, sorted by timestamp.

