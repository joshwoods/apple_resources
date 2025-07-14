

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.InputSource 

Class

# AVCaptureDevice.InputSource

A distinct input source on a capture device.

macOS 10.7+

``` source
class InputSource
```

## Overview

A capture device may optionally present an array of input sources that represent distinct mutually exclusive inputs to the device. For example, an audio capture device might have ADAT optical and analog input sources; a video capture device might have an HDMI or component input source.

## Topics

### Accessing Properties

var inputSourceID: String

An identifier for an input source.

var localizedName: String

A localized, human-readable name for the input source.

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

### Configuring Input Sources

var inputSources: [AVCaptureDevice.InputSource]

An array of input sources that the device supports.

var activeInputSource: AVCaptureDevice.InputSource?

The currently active input source of the device.

