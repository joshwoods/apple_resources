

- AVFoundation
- AVAssetImageGenerator
-  customVideoCompositor 

Instance Property

# customVideoCompositor

A custom video compositor to use when extracting images from assets with multiple video tracks.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var customVideoCompositor: (any AVVideoCompositing)? { get }
```

## See Also

### Configuring Compositing

var videoComposition: AVVideoComposition?

A video composition to use when extracting images from assets with multiple video tracks.

