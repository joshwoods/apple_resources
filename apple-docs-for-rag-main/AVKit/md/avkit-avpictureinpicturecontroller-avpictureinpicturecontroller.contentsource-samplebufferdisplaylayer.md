

- AVKit
- AVPictureInPictureController
- AVPictureInPictureController.ContentSource
-  sampleBufferDisplayLayer 

Instance Property

# sampleBufferDisplayLayer

The presenting sample buffer display layer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var sampleBufferDisplayLayer: AVSampleBufferDisplayLayer? { get }
```

## Discussion

This value is `nil` if the content source doesn’t represent a sample buffer display layer.

## See Also

### Accessing the Presentation Layer

var playerLayer: AVPlayerLayer?

The presenting player layer.

