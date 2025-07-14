

- AVFoundation
-  AVCaptureSystemExposureBiasSlider 

Class

# AVCaptureSystemExposureBiasSlider

A control that adjusts the exposure bias of a capture device within the system-recommended range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
class AVCaptureSystemExposureBiasSlider
```

## Mentioned in 

Enhancing your app experience with the Camera Control

## Overview

This control defines its range by querying the systemRecommendedExposureBiasRange property of the device’s active format. If a device’s activeFormat value changes, the slider updates its range with the new format’s system-recommended value.

To use this control, add it to the capture session by calling the session’s addControl(_:) method.

## Topics

### Creating an exposure bias slider

init(device: AVCaptureDevice)

Creates a slider to control the exposure bias of the specified capture device.

init(device: AVCaptureDevice, action: (Float) -> Void)

Creates a slider to control the exposure bias of the specified capture device with an action to respond to exposure bias changes.

## Relationships

### Inherits From

- AVCaptureControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Capture controls

Enhancing your app experience with the Camera Control

Provide direct access to your camera app’s features to help people quickly capture the perfect shot.

class AVCaptureControl

An abstract base class for controls that interact with the camera system.

class AVCaptureSystemZoomSlider

A control that adjusts the video zoom factor of a capture device within the system-recommended range.

class AVCaptureSlider

A slider control that selects a value from a bounded range.

class AVCaptureIndexPicker

A control for selecting from a set of mutually exclusive values by index.

