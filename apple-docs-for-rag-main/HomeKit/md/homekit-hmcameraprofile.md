

- HomeKit
-  HMCameraProfile 

Class

# HMCameraProfile

A camera profile that interacts with an accessory’s camera.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class HMCameraProfile
```

## Overview

Each profile control is optional, because an individual camera vendor may not support all of the features defined by the HomeKit camera specifications.

## Topics

### Controlling camera settings

var settingsControl: HMCameraSettingsControl?

Controls the settings on the camera.

class HMCameraSettingsControl

An object that represents the ability to control a camera’s settings.

class HMCameraControl

An abstract class that represents a camera control.

### Playing audio

var microphoneControl: HMCameraAudioControl?

Controls the microphone settings on the camera.

var speakerControl: HMCameraAudioControl?

Controls the speaker settings on the camera.

class HMCameraAudioControl

An object that controls a camera’s audio settings.

### Streaming

var streamControl: HMCameraStreamControl?

Controls the camera stream.

class HMCameraStreamControl

An object that can start and stop the camera stream and contains the view into which the stream is rendered.

### Capturing snapshots

var snapshotControl: HMCameraSnapshotControl?

Controls the camera’s snapshot function.

class HMCameraSnapshotControl

An object that can take an image snapshot from a camera.

## Relationships

### Inherits From

- HMAccessoryProfile

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Managing accessory profiles

var profiles: [HMAccessoryProfile]

An array of profiles implemented by the accessory.

class HMAccessoryProfile

A profile that certain accessories implement.

class HMNetworkConfigurationProfile

A profile that provides information about network protection for an accessory.

