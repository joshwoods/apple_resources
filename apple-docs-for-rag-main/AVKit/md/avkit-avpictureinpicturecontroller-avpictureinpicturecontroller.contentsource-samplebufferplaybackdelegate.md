

- AVKit
- AVPictureInPictureController
- AVPictureInPictureController.ContentSource
-  sampleBufferPlaybackDelegate 

Instance Property

# sampleBufferPlaybackDelegate

A delegate object that responds to sample buffer playback events.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
weak var sampleBufferPlaybackDelegate: (any AVPictureInPictureSampleBufferPlaybackDelegate)? { get }
```

## See Also

### Configuring the Delegate

protocol AVPictureInPictureSampleBufferPlaybackDelegate

A protocol for controlling playback from a sample buffer display layer in Picture in Picture.

