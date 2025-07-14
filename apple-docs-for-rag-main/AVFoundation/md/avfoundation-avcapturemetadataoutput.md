

- AVFoundation
-  AVCaptureMetadataOutput 

Class

# AVCaptureMetadataOutput

A capture output for processing timed metadata produced by a capture session.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
class AVCaptureMetadataOutput
```

## Overview

An `AVCaptureMetadataOutput` object intercepts metadata objects emitted by its associated capture connection and forwards them to a delegate object for processing. You can use instances of this class to process specific types of metadata included with the input data. You use this class the way you do other output objects, typically by adding it as an output to an AVCaptureSession object.

## Topics

### Configuring Metadata Capture

var availableMetadataObjectTypes: [AVMetadataObject.ObjectType]

An array of strings identifying the types of metadata objects that can be captured.

var metadataObjectTypes: [AVMetadataObject.ObjectType]!

An array of strings identifying the types of metadata objects to process.

var rectOfInterest: CGRect

A rectangle of interest for limiting the search area for visual metadata.

### Receiving Captured Metadata Objects

func setMetadataObjectsDelegate((any AVCaptureMetadataOutputObjectsDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue to use handle callbacks.

var metadataObjectsDelegate: (any AVCaptureMetadataOutputObjectsDelegate)?

The delegate of the capture metadata output object.

var metadataObjectsCallbackQueue: dispatch_queue_t?

The dispatch queue on which to execute the delegate’s methods.

protocol AVCaptureMetadataOutputObjectsDelegate

Methods for receiving metadata produced by a metadata capture output.

### Creating Metadata Output

init()

Creates a new capture metadata output.

## Relationships

### Inherits From

- AVCaptureOutput

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

class AVMetadataObject

The abstract superclass for objects provided by a metadata capture output.

Metadata Types

Inspect the supported metadata object types that the framework supports.

