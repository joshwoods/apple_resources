

- AVFoundation
- AVAssetReaderVideoCompositionOutput
-  customVideoCompositor 

Instance Property

# customVideoCompositor

A custom video compositor for the output.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var customVideoCompositor: (any AVVideoCompositing)? { get }
```

## Discussion

This property is `nil` if there isn’t a custom video compositor, or if the internal video compositor is in use.

## See Also

### Configuring Video Settings

var videoComposition: AVVideoComposition?

The video composition to use for the output.

