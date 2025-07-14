

- AVFoundation
-  AVCaptureMetadataInput 

Class

# AVCaptureMetadataInput

A capture input for providing timed metadata to a capture session.

iOS 9.0+iPadOS 9.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureMetadataInput
```

## Overview

This class provides input to an AVCaptureSession. An instance of AVCaptureMetadataInput can present one and only one AVCaptureInput.Port connected to an AVCaptureMovieFileOutput. Provide metadata through the input port by conforming to a doc://com.apple.documentation/documentation/coremedia/cmformatdescription-u8g and supplying AVMetadataItem objects in an AVTimedMetadataGroup.

## Topics

### Creating Metadata Input

init(formatDescription: CMMetadataFormatDescription, clock: CMClock)

Creates capture metadata input to provide timed groups to a capture session.

### Providing Metadata

func append(AVTimedMetadataGroup) throws

Provides metadata to the capture session.

## Relationships

### Inherits From

- AVCaptureInput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Metadata capture

class AVCaptureMetadataOutput

A capture output for processing timed metadata produced by a capture session.

class AVMetadataObject

The abstract superclass for objects provided by a metadata capture output.

Metadata Types

Inspect the supported metadata object types that the framework supports.

