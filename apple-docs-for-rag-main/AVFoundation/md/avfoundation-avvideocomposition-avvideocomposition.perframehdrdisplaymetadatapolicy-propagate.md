

- AVFoundation
- AVVideoComposition
- AVVideoComposition.PerFrameHDRDisplayMetadataPolicy
-  propagate 

Type Property

# propagate

A policy that passes HDR metadata through, if present on the composed frame.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static let propagate: AVVideoComposition.PerFrameHDRDisplayMetadataPolicy
```

## See Also

### Policies

static let generate: AVVideoComposition.PerFrameHDRDisplayMetadataPolicy

A video composition may generate HDR metadata and attach it to the rendered frame.

