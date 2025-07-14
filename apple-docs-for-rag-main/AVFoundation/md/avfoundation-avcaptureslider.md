

- AVFoundation
-  AVCaptureSlider 

Class

# AVCaptureSlider

A slider control that selects a value from a bounded range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
class AVCaptureSlider
```

## Mentioned in 

Enhancing your app experience with the Camera Control

## Overview

Sliders are appropriate for controls that provide a single float value.

## Topics

### Creating a slider

convenience init(String, symbolName: String, in: ClosedRange&lt;Float>)

Creates a continuous slider control that selects a value from a bounded range.

convenience init(String, symbolName: String, in: ClosedRange&lt;Float>, step: Float)

Creates a discrete slider control that selects a stepped value from a bounded range.

convenience init(String, symbolName: String, values: [Float])

Creates a discrete slider control that selects a value from a list.

### Handling interaction

func setActionQueue(DispatchQueue, action: (Float) -> ())

Sets the action to perform on the specified dispatch queue when the control’s value changes.

### Accessing the control value

var value: Float

The current value of the slider.

var prominentValues: [Float]

Values in this array may receive unique visual representations or behaviors.

var localizedValueFormat: String?

A localized string that defines the presentation of the slider’s value.

### Setting an accessibility identifier

var accessibilityIdentifier: String?

A string identifier for the slider.

### Inspecting presentation attributes

var symbolName: String

The name of the SF Symbol that represents this control.

var localizedTitle: String

A localized title that describes the control’s action.

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

class AVCaptureSystemExposureBiasSlider

A control that adjusts the exposure bias of a capture device within the system-recommended range.

class AVCaptureIndexPicker

A control for selecting from a set of mutually exclusive values by index.

