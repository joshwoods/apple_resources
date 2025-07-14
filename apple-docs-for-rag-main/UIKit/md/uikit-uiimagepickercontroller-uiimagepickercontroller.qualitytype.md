

- UIKit
- UIImagePickerController
-  UIImagePickerController.QualityType 

Enumeration

# UIImagePickerController.QualityType

Constants that describe video quality settings for movies that are recorded with the built-in camera, or that are transcoded when they’re displayed in the image picker.

iOSiPadOSMac Catalyst

``` source
enum QualityType
```

## Overview

The constants in this enumeration are for use as values of the videoQuality property.

The video quality setting applies to transcoding as well as to recording. Specifically, if the video quality setting is lower than the video quality of an existing movie, displaying that movie in the picker results in transcoding the movie to the lower quality.

## Topics

### Constants

case typeHigh

If recording, specifies that you want to use the highest-quality video recording supported for the active camera on the device.

case type640x480

If recording, specifies that you want to use VGA-quality video recording (pixel dimensions of 640x480).

case typeMedium

If recording, specifies that you want to use medium-quality video recording.

case typeLow

If recording, specifies that you want to use low-quality video recording.

case typeIFrame1280x720

If recording, specifies that you want to use 1280x720 iFrame format.

case typeIFrame960x540

If recording, specifies that you want to use 960x540 iFrame format.

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

### Configuring the video capture options

var videoQuality: UIImagePickerController.QualityType

The video recording and transcoding quality.

var videoMaximumDuration: TimeInterval

The maximum duration, in seconds, for a video recording.

