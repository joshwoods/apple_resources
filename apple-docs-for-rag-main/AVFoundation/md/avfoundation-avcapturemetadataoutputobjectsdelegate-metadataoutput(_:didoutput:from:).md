

- AVFoundation
- AVCaptureMetadataOutputObjectsDelegate
-  metadataOutput(\_:didOutput:from:) 

Instance Method

# metadataOutput(\_:didOutput:from:)

Informs the delegate that the capture output object emitted new metadata objects.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
optional func metadataOutput(
    _ output: AVCaptureMetadataOutput,
    didOutput metadataObjects: [AVMetadataObject],
    from connection: AVCaptureConnection
)
```

## Parameters 

`output`  

The AVCaptureMetadataOutput object that captured and emitted the metadata objects.

`metadataObjects`  

An array of AVMetadataObject instances representing the newly emitted metadata. Because AVMetadataObject is an abstract class, the objects in this array are always instances of a concrete subclass.

`connection`  

The capture connection through which the objects were emitted.

## Discussion

The AVCaptureMetadataOutput object emits only metadata objects whose types are included in its metadataObjectTypes property. The delegate implements this method to perform additional processing on metadata objects as they become available. If you plan to use metadata objects outside the scope of this method, you must store strong references to them and remove those references when the objects are no longer required.

This method is executed on the dispatch queue specified by the metadataObjectsCallbackQueue property of the capture metadata output object. Because this method may be called frequently, your implementation should be efficient to prevent capture performance problems, including dropped metadata objects.

