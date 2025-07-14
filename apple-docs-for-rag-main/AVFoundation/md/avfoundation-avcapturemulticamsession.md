

- AVFoundation
-  AVCaptureMultiCamSession 

Class

# AVCaptureMultiCamSession

A capture session that supports simultaneous capture from multiple inputs of the same media type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 2.1+

``` source
class AVCaptureMultiCamSession
```

## Overview

The session preset for a multicamera session is always inputPriority. Set each capture device’s activeFormat value to the desired quality of service.

You can dynamically enable and disable this session’s individual camera inputs without interrupting capture preview. To stop an individual camera, disable all of its connections or connected ports. The camera then stops streaming data to save power and bandwidth. Other inputs that are streaming data through the session are unaffected.

Note

If your app only needs to capture from a single camera at a time, use AVCaptureSession instead.

## Topics

### Determining Multi-Camera Support

class var isMultiCamSupported: Bool

A Boolean value that indicates whether this device supports multi-camera sessions.

### Managing Resources

var hardwareCost: Float

A value that indicates the percentage of the session’s available hardware budget currently in use.

var systemPressureCost: Float

A value that indicates the system pressure cost of the current session configuration.

## Relationships

### Inherits From

- AVCaptureSession

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Capture sessions

Setting Up a Capture Session

Configure input devices, output media, preview views, and basic settings before capturing photos or video.

Accessing the camera while multitasking on iPad

Operate the camera in Split View, Slide Over, Picture in Picture, and Stage Manager modes.

AVCam: Building a camera app

Capture photos and record video using the front and rear iPhone and iPad cameras.

AVMultiCamPiP: Capturing from Multiple Cameras

Simultaneously record the output from the front and back cameras into a single movie file by using a multi-camera capture session.

AVCamBarcode: Detecting Barcodes and Faces

Identify machine readable codes or faces by using the camera.

class AVCaptureSession

An object that configures capture behavior and coordinates the flow of data from input devices to capture outputs.

class AVCaptureInput

An abstract superclass for objects that provide input data to a capture session.

class AVCaptureOutput

An abstract superclass for objects that provide media output destinations for a capture session.

class AVCaptureConnection

An object that represents a connection from a capture input to a capture output.

