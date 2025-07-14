

- AVFoundation
-  AVCaptureControl 

Class

# AVCaptureControl

An abstract base class for controls that interact with the camera system.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
class AVCaptureControl
```

## Mentioned in 

Enhancing your app experience with the Camera Control

## Overview

Capture controls provide the interface for interacting with the camera system from the Camera Control button on iPhone 16 devices. The framework provides several concrete subclasses of this class that allow apps to access built-in functionality and define custom controls.

## Topics

### Setting the enabled state

var isEnabled: Bool

A Boolean value that indicates whether this control supports user interaction.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCaptureIndexPicker
- AVCaptureSlider
- AVCaptureSystemExposureBiasSlider
- AVCaptureSystemZoomSlider

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

class AVCaptureSystemZoomSlider

A control that adjusts the video zoom factor of a capture device within the system-recommended range.

class AVCaptureSystemExposureBiasSlider

A control that adjusts the exposure bias of a capture device within the system-recommended range.

class AVCaptureSlider

A slider control that selects a value from a bounded range.

class AVCaptureIndexPicker

A control for selecting from a set of mutually exclusive values by index.

