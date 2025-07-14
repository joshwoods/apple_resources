

- UIKit
-  UIDeviceOrientation 

Enumeration

# UIDeviceOrientation

Constants that describe the physical orientation of the device.

iOSiPadOSMac CatalystvisionOS

``` source
enum UIDeviceOrientation
```

## Overview

The orientation property uses these constants to identify the device orientation. These constants identify the physical orientation of the device and aren’t tied to the orientation of your app’s user interface.

## Topics

### Device orientations

case unknown

The orientation of the device can’t be determined.

case portrait

The device is in portrait mode, with the device held upright and the front-facing camera at the top.

case portraitUpsideDown

The device is in portrait mode but upside down, with the device held upright and the front-facing camera at the bottom.

case landscapeLeft

The device is in landscape mode, with the device held upright and the front-facing camera on the left side.

case landscapeRight

The device is in landscape mode, with the device held upright and the front-facing camera on the right side.

case faceUp

The device is held parallel to the ground with the screen facing upwards.

case faceDown

The device is held parallel to the ground with the screen facing downwards.

### Orientation testing

var isPortrait: Bool

A Boolean value that indicates whether the device is in a portrait orientation.

var isLandscape: Bool

A Boolean value that indicates whether the device is in a landscape orientation.

var isFlat: Bool

A Boolean value that indicates whether the specified orientation is face up or face down.

var isValidInterfaceOrientation: Bool

A Boolean value that indicates whether the specified orientation is one of the portrait or landscape orientations.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Tracking the device orientation

var orientation: UIDeviceOrientation

The physical orientation of the device.

var isGeneratingDeviceOrientationNotifications: Bool

A Boolean value that indicates whether the device generates orientation notifications.

func beginGeneratingDeviceOrientationNotifications()

Begins the generation of notifications of device orientation changes.

func endGeneratingDeviceOrientationNotifications()

Ends the generation of notifications of device orientation changes.

