

- AVFoundation
- AVCaptureMetadataOutput
-  metadataObjectsDelegate 

Instance Property

# metadataObjectsDelegate

The delegate of the capture metadata output object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
var metadataObjectsDelegate: (any AVCaptureMetadataOutputObjectsDelegate)? { get }
```

## Discussion

The delegate object must conform to the AVCaptureMetadataOutputObjectsDelegate protocol. The object in this property is used to process all metadata objects captured from the capture metadata output object’s connection.

To set the delegate object, you must use the setMetadataObjectsDelegate(_:queue:) method.

## See Also

### Receiving Captured Metadata Objects

func setMetadataObjectsDelegate((any AVCaptureMetadataOutputObjectsDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue to use handle callbacks.

var metadataObjectsCallbackQueue: dispatch_queue_t?

The dispatch queue on which to execute the delegate’s methods.

protocol AVCaptureMetadataOutputObjectsDelegate

Methods for receiving metadata produced by a metadata capture output.

