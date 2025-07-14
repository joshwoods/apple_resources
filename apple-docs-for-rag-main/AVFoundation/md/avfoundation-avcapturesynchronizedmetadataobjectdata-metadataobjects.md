

- AVFoundation
- AVCaptureSynchronizedMetadataObjectData
-  metadataObjects 

Instance Property

# metadataObjects

The list of metadata objects captured at this synchronization timestamp.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var metadataObjects: [AVMetadataObject] { get }
```

## Discussion

Note

Because AVMetadataObject is an abstract class, the objects in this array are always instances of a concrete subclass.

This array is equivalent to that provided by the metadataOutput(_:didOutput:from:) delegate method when using a metadata capture output without a data output synchronizer.

