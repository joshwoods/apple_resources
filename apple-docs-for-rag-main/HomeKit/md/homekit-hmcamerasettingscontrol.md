

- HomeKit
-  HMCameraSettingsControl 

Class

# HMCameraSettingsControl

An object that represents the ability to control a camera’s settings.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class HMCameraSettingsControl
```

## Topics

### Controlling camera characteristics

var currentHorizontalTilt: HMCharacteristic?

Characteristic corresponding to the camera’s current horizontal tilt setting.

var targetHorizontalTilt: HMCharacteristic?

Characteristic corresponding to adjusting the camera’s horizontal tilt setting.

var currentVerticalTilt: HMCharacteristic?

Characteristic corresponding to the camera’s current vertical tilt setting.

var targetVerticalTilt: HMCharacteristic?

Characteristic corresponding to adjusting the camera’s vertical tilt setting.

var opticalZoom: HMCharacteristic?

Characteristic corresponding to the camera’s optical zoom setting.

var digitalZoom: HMCharacteristic?

Characteristic corresponding to the camera’s digital zoom setting.

var imageMirroring: HMCharacteristic?

Characteristic corresponding to the camera’s image mirroring setting.

var imageRotation: HMCharacteristic?

Characteristic corresponding to the camera’s image rotation setting.

var nightVision: HMCharacteristic?

Characteristic corresponding to the camera’s night vision setting.

## Relationships

### Inherits From

- HMCameraControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Controlling camera settings

var settingsControl: HMCameraSettingsControl?

Controls the settings on the camera.

class HMCameraControl

An abstract class that represents a camera control.

