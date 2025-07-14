

- AVKit
- AVPlayerViewPictureInPictureDelegate
-  playerViewWillStopPicture(inPicture:) 

Instance Method

# playerViewWillStopPicture(inPicture:)

Tells the delegate that Picture in Picture playback is about to stop.

macOS 10.15+

``` source
optional func playerViewWillStopPicture(inPicture playerView: AVPlayerView)
```

## Parameters 

`playerView`  

The player view.

## See Also

### Responding to Picture in Picture Playback Events

func playerViewWillStartPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback is about to start.

func playerViewDidStartPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback started.

func playerViewDidStopPicture(inPicture: AVPlayerView)

Tells the delegate that Picture in Picture playback stopped.

func playerView(AVPlayerView, failedToStartPictureInPictureWithError: any Error)

Tells the delegate that Picture in Picture playback failed to start.

func playerView(AVPlayerView, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the user interface before Picture in Picture playback stops.

func playerViewShouldAutomaticallyDismissAtPicture(inPictureStart: AVPlayerView) -> Bool

Asks the delegate if the player view should miniaturize when Picture in Picture starts.

