

- AVKit
-  AVPlayerViewPictureInPictureDelegate 

Protocol

# AVPlayerViewPictureInPictureDelegate

A protocol that defines the methods to implement to respond to Picture in Picture playback events.

macOS 10.15+

``` source
protocol AVPlayerViewPictureInPictureDelegate : NSObjectProtocol
```

## Topics

### Responding to Picture in Picture Playback Events

func playerViewWillStartPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback is about to start.

func playerViewDidStartPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback started.

func playerViewWillStopPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback is about to stop.

func playerViewDidStopPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback stopped.

func playerView(AVPlayerView, failedToStartPictureInPictureWithError: any Error)

Tells the delegate that Picture in Picture playback failed to start.

func playerView(AVPlayerView, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the user interface before Picture in Picture playback stops.

func playerViewShouldAutomaticallyDismissAtPicture(inPictureStart: AVPlayerView) -> Bool

Asks the delegate if the player view should miniaturize when Picture in Picture starts.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring Picture in Picture

var allowsPictureInPicturePlayback: Bool

A Boolean value that determines whether the player view allows Picture in Picture playback.

var pictureInPictureDelegate: (any AVPlayerViewPictureInPictureDelegate)?

The Picture in Picture delegate object.

