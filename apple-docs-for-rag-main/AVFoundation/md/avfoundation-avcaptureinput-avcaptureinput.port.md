

- AVFoundation
- AVCaptureInput
-  AVCaptureInput.Port 

Class

# AVCaptureInput.Port

An object that represents a stream of data that a capture input provides.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
class Port
```

## Overview

Instances of AVCaptureInput have one or more input ports, one for each data stream they can produce. For example, an AVCaptureDeviceInput object presenting one video data stream has one port.

## Topics

### Inspecting an Input Port

var isEnabled: Bool

A Boolean value that indicates whether the port is in an enabled state.

var mediaType: AVMediaType

The media type of the port.

var formatDescription: CMFormatDescription?

A description of the port format.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The device type of the source camera that provides data to the port.

var sourceDevicePosition: AVCaptureDevice.Position

The position of the source device providing input through this port.

var clock: CMClock?

An object that represents the capture device’s clock.

### Observing Format Changes

class let formatDescriptionDidChangeNotification: NSNotification.Name

A notification the system posts when the capture input port’s format description changes.

### Accessing the Input

var input: AVCaptureInput

The input object that owns the port.

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

### Accessing Ports

var ports: [AVCaptureInput.Port]

The ports available on a capture input.

