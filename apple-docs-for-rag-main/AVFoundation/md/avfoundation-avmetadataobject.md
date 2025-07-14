

- AVFoundation
-  AVMetadataObject 

Class

# AVMetadataObject

The abstract superclass for objects provided by a metadata capture output.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.10+tvOS 9.0+

``` source
class AVMetadataObject
```

## Overview

The `AVMetadataObject` class is an abstract class that defines the basic properties associated with a piece of metadata. These attributes reflect information either about the metadata itself or the media from which the metadata originated. Subclasses are responsible for providing appropriate values for each of the relevant properties.

You shouldn’t subclass `AVMetadataObject` directly. Instead, you use one of the defined subclasses provided by the AVFoundation framework. Similarly, you don’t create instances of this class yourself but use an AVCaptureMetadataOutput object to retrieve them from the captured data.

## Topics

### Getting the Type of Metadata

var type: AVMetadataObject.ObjectType

The type of metadata that this object provides.

struct ObjectType

Constants that identify metadata object types.

### Getting the Media-Related Attributes

var time: CMTime

The media time value associated with the metadata object.

var duration: CMTime

The duration of the media associated with this metadata object.

var bounds: CGRect

The bounding rectangle associated with the metadata.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMetadataBodyObject
- AVMetadataFaceObject
- AVMetadataMachineReadableCodeObject
- AVMetadataSalientObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Metadata capture

class AVCaptureMetadataInput

A capture input for providing timed metadata to a capture session.

class AVCaptureMetadataOutput

A capture output for processing timed metadata produced by a capture session.

Metadata Types

Inspect the supported metadata object types that the framework supports.

