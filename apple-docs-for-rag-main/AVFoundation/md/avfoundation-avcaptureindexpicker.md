

- AVFoundation
-  AVCaptureIndexPicker 

Class

# AVCaptureIndexPicker

A control for selecting from a set of mutually exclusive values by index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
class AVCaptureIndexPicker
```

## Mentioned in 

Enhancing your app experience with the Camera Control

## Overview

Index pickers are appropriate for controls that provide an indexed container of values.

## Topics

### Creating an index picker

init(String, symbolName: String, numberOfIndexes: Int)

Creates a control to pick a value from the specified number of indexes.

init(String, symbolName: String, numberOfIndexes: Int, localizedTitleTransform: (Int) -> String)

Creates a control to pick a value from the specified number of indices.

init(String, symbolName: String, localizedIndexTitles: [String])

Creates an object to select an index from a set of values.

### Handling interaction

func setActionQueue(DispatchQueue, action: (Int) -> ())

Sets the action to perform on the specified dispatch queue when the control’s value changes.

### Accessing the control value

var selectedIndex: Int

The currently selected index.

var numberOfIndexes: Int

The number of index values the control provides.

### Setting an accessibility identifier

var accessibilityIdentifier: String?

A string identifier for this control.

### Inspecting presentation attributes

var symbolName: String

The name of the SF Symbol that represents this control.

var localizedTitle: String

A localized title that describes the control’s action.

var localizedIndexTitles: [String]

The titles to present for each index.

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

class AVCaptureSlider

A slider control that selects a value from a bounded range.

