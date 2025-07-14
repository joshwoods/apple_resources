

- AVFoundation
-  AVCaptureInput 

Class

# AVCaptureInput

An abstract superclass for objects that provide input data to a capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class AVCaptureInput
```

## Mentioned in 

Setting Up a Capture Session

## Overview

You create concrete instances of this class, such as AVCaptureDeviceInput, to add inputs to a capture session. An input provides one or more streams of media data. For example, input devices can provide both audio and video data. The framework represents each media stream that an input provides as an AVCaptureInput.Port object.

A capture makes connections between capture inputs and capture outputs using a AVCaptureConnection object. The connection defines the mapping between a set of port objects and an AVCaptureOutput.

## Topics

### Accessing Ports

var ports: [AVCaptureInput.Port]

The ports available on a capture input.

class Port

An object that represents a stream of data that a capture input provides.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCaptureDeviceInput
- AVCaptureMetadataInput
- AVCaptureScreenInput

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

class AVCaptureMultiCamSession

A capture session that supports simultaneous capture from multiple inputs of the same media type.

class AVCaptureOutput

An abstract superclass for objects that provide media output destinations for a capture session.

class AVCaptureConnection

An object that represents a connection from a capture input to a capture output.

