

- AVFoundation
-  AVCaptureOutput 

Class

# AVCaptureOutput

An abstract superclass for objects that provide media output destinations for a capture session.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class AVCaptureOutput
```

## Mentioned in 

Setting Up a Capture Session

## Overview

This class provides an abstract interface to connect capture output destinations, such as files and streams, to a capture session.

A capture output can have multiple connections, one for each stream of media that it receives from a capture input. A capture output doesn’t have any connections when you create it. When you add it to a capture session, the session automatically forms connections between compatible inputs and outputs.

## Topics

### Accessing Connections

var connections: [AVCaptureConnection]

The capture output object’s connections.

func connection(with: AVMediaType) -> AVCaptureConnection?

Returns the first connection with an input port of a specified media type.

enum DataDroppedReason

Constants that define reasons for why the system dropped a frame.

### Converting Between Coordinate Systems

func transformedMetadataObject(for: AVMetadataObject, connection: AVCaptureConnection) -> AVMetadataObject?

Converts a metadata object’s visual properties to layer coordinates.

func metadataOutputRectConverted(fromOutputRect: CGRect) -> CGRect

Converts a rectangle in the capture output object’s coordinate system to one in the coordinate system used for metadata outputs.

func outputRectConverted(fromMetadataOutputRect: CGRect) -> CGRect

Converts a rectangle in the coordinate system used for metadata outputs to one in the capture output object’s coordinate system.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCaptureAudioDataOutput
- AVCaptureAudioPreviewOutput
- AVCaptureDepthDataOutput
- AVCaptureFileOutput
- AVCaptureMetadataOutput
- AVCapturePhotoOutput
- AVCaptureStillImageOutput
- AVCaptureVideoDataOutput

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

class AVCaptureInput

An abstract superclass for objects that provide input data to a capture session.

class AVCaptureConnection

An object that represents a connection from a capture input to a capture output.

