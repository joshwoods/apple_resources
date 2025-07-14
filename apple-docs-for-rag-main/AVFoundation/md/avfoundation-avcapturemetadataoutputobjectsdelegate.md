

- AVFoundation
-  AVCaptureMetadataOutputObjectsDelegate 

Protocol

# AVCaptureMetadataOutputObjectsDelegate

Methods for receiving metadata produced by a metadata capture output.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
protocol AVCaptureMetadataOutputObjectsDelegate : NSObjectProtocol
```

## Overview

The `AVCaptureMetadataOutputObjectsDelegate` protocol must be adopted by the delegate of an AVCaptureMetadataOutput object. The single method in this protocol is optional. The method allows a delegate to respond when a capture metadata output object receives relevant metadata objects through its connection.

The AVCaptureMetadataOutput object calls the methods of the delegate object on the dispatch queue associated with its metadataObjectsCallbackQueue property.

## Topics

### Processing Emitted Metadata Objects

func metadataOutput(AVCaptureMetadataOutput, didOutput: [AVMetadataObject], from: AVCaptureConnection)

Informs the delegate that the capture output object emitted new metadata objects.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Receiving Captured Metadata Objects

func setMetadataObjectsDelegate((any AVCaptureMetadataOutputObjectsDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue to use handle callbacks.

var metadataObjectsDelegate: (any AVCaptureMetadataOutputObjectsDelegate)?

The delegate of the capture metadata output object.

var metadataObjectsCallbackQueue: dispatch_queue_t?

The dispatch queue on which to execute the delegate’s methods.

