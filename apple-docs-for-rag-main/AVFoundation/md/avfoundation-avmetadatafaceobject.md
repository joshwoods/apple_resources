

- AVFoundation
-  AVMetadataFaceObject 

Class

# AVMetadataFaceObject

Face information detected by a metadata capture output.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.10+tvOS 9.0+

``` source
class AVMetadataFaceObject
```

## Mentioned in 

Configuring Camera Capture to Collect a Portrait Effects Matte

## Overview

The `AVMetadataFaceObject` class is a concrete subclass of AVMetadataObject that defines the features of a single detected face. You can retrieve instances of this class from the output of an AVCaptureMetadataOutput object on devices that support face detection.

## Topics

### Getting the Face Identifier

var faceID: Int

The unique ID for this face metadata object.

### Accessing the Face Detection Data

var hasRollAngle: Bool

A Boolean value indicating whether there is a valid roll angle associated with the face.

var rollAngle: CGFloat

The roll angle of the face specified in degrees.

var hasYawAngle: Bool

A Boolean value indicating whether there is a valid yaw angle associated with the face.

var yawAngle: CGFloat

The yaw angle of the face specified in degrees.

### Constants

Face Metadata Type

A metadata type string for face detection metadata.

## Relationships

### Inherits From

- AVMetadataObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

