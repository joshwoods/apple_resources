

- AVKit
- AVPictureInPictureController
-  AVPictureInPictureController.ContentSource 

Class

# AVPictureInPictureController.ContentSource

An object that represents the source of the content to present in Picture in Picture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class ContentSource
```

## Mentioned in 

Adopting Picture in Picture for video calls

## Overview

The system supports displaying content from an AVPlayerLayer or AVSampleBufferDisplayLayer in a Picture in Picture window. Use an instance of this class to describe the source of your app’s content.

## Topics

### Creating a Content Source

init(playerLayer: AVPlayerLayer)

Creates a content source with a player layer.

init(sampleBufferDisplayLayer: AVSampleBufferDisplayLayer, playbackDelegate: any AVPictureInPictureSampleBufferPlaybackDelegate)

Creates a content source with a sample buffer display layer.

init(activeVideoCallSourceView: UIView, contentViewController: AVPictureInPictureVideoCallViewController)

Creates a content source with an active video call.

### Accessing the Presentation Layer

var playerLayer: AVPlayerLayer?

The presenting player layer.

var sampleBufferDisplayLayer: AVSampleBufferDisplayLayer?

The presenting sample buffer display layer.

### Accessing the Active Call Presentation

var activeVideoCallSourceView: UIView?

The view that contains the video content of the call.

var activeVideoCallContentViewController: AVPictureInPictureVideoCallViewController

The view controller that presents the video call content.

class AVPictureInPictureVideoCallViewController

A view controller that presents content from a video call in Picture in Picture.

### Configuring the Delegate

var sampleBufferPlaybackDelegate: (any AVPictureInPictureSampleBufferPlaybackDelegate)?

A delegate object that responds to sample buffer playback events.

protocol AVPictureInPictureSampleBufferPlaybackDelegate

A protocol for controlling playback from a sample buffer display layer in Picture in Picture.

### Invalidating State

func invalidatePlaybackState()

Invalidates the controller’s current playback state and fetches the updated state from the sample buffer playback delegate object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuring the Content Source

var contentSource: AVPictureInPictureController.ContentSource?

The source of the controller’s content.

