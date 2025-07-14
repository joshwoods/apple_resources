

- AVFoundation
- AVAssetWriterInput
-  metadata 

Instance Property

# metadata

The track-level metadata to write to the output.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var metadata: [AVMetadataItem] { get set }
```

## Discussion

You can’t set this property after writing starts.

