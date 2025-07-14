

- AVFoundation
- AVCaptureMetadataOutput
-  metadataObjectsCallbackQueue 

Instance Property

# metadataObjectsCallbackQueue

The dispatch queue on which to execute the delegate’s methods.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
var metadataObjectsCallbackQueue: dispatch_queue_t? { get }
```

## Discussion

To set the dispatch queue, you must use the setMetadataObjectsDelegate(_:queue:) method.

## See Also

### Receiving Captured Metadata Objects

func setMetadataObjectsDelegate((any AVCaptureMetadataOutputObjectsDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue to use handle callbacks.

var metadataObjectsDelegate: (any AVCaptureMetadataOutputObjectsDelegate)?

The delegate of the capture metadata output object.

protocol AVCaptureMetadataOutputObjectsDelegate

Methods for receiving metadata produced by a metadata capture output.

