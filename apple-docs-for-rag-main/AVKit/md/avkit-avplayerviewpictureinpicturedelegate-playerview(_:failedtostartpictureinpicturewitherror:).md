

- AVKit
- AVPlayerViewPictureInPictureDelegate
-  playerView(\_:failedToStartPictureInPictureWithError:) 

Instance Method

# playerView(\_:failedToStartPictureInPictureWithError:)

Tells the delegate that Picture in Picture playback failed to start.

macOS 10.15+

``` source
optional func playerView(
    _ playerView: AVPlayerView,
    failedToStartPictureInPictureWithError error: any Error
)
```

## Parameters 

`playerView`  

The player view.

`error`  

An error object describing the failure.

## See Also

### Responding to Picture in Picture Playback Events

func playerViewWillStartPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback is about to start.

func playerViewDidStartPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback started.

func playerViewWillStopPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback is about to stop.

func playerViewDidStopPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback stopped.

func playerView(AVPlayerView, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the user interface before Picture in Picture playback stops.

func playerViewShouldAutomaticallyDismissAtPicture(inPictureStart: AVPlayerView) -> Bool

Asks the delegate if the player view should miniaturize when Picture in Picture starts.

