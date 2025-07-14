

- AVKit
- AVPictureInPictureController
- AVPictureInPictureController.ContentSource
-  playerLayer 

Instance Property

# playerLayer

The presenting player layer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var playerLayer: AVPlayerLayer? { get }
```

## Discussion

This value is `nil` if the content source doesn’t represent a player layer.

## See Also

### Accessing the Presentation Layer

var sampleBufferDisplayLayer: AVSampleBufferDisplayLayer?

The presenting sample buffer display layer.

