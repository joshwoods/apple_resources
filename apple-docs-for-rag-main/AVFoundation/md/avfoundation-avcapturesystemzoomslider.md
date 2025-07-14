

- AVFoundation
-  AVCaptureSystemZoomSlider 

Class

# AVCaptureSystemZoomSlider

A control that adjusts the video zoom factor of a capture device within the system-recommended range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
class AVCaptureSystemZoomSlider
```

## Mentioned in 

Enhancing your app experience with the Camera Control

## Overview

The system sets the slider’s range to the value of the systemRecommendedVideoZoomRange property of the device’s active format. If a device’s activeFormat value changes, the slider updates its range to the new format’s recommendation.

To use this control, add it to the capture session by calling the session’s addControl(_:) method.

## Topics

### Creating a zoom slider

init(device: AVCaptureDevice)

Creates a slider to control the video zoom factor of a capture device.

init(device: AVCaptureDevice, action: (CGFloat) -> Void)

Creates a slider to control the zoom level of the specified capture device with an action to respond to zoom changes.

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

class AVCaptureSystemExposureBiasSlider

A control that adjusts the exposure bias of a capture device within the system-recommended range.

class AVCaptureSlider

A slider control that selects a value from a bounded range.

class AVCaptureIndexPicker

A control for selecting from a set of mutually exclusive values by index.

