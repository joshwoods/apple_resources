

- AVKit
- AVPlayerViewPictureInPictureDelegate
-  playerViewShouldAutomaticallyDismissAtPicture(inPictureStart:) 

Instance Method

# playerViewShouldAutomaticallyDismissAtPicture(inPictureStart:)

Asks the delegate if the player view should miniaturize when Picture in Picture starts.

macOS 10.15+

``` source
optional func playerViewShouldAutomaticallyDismissAtPicture(inPictureStart playerView: AVPlayerView) -> Bool
```

## Parameters 

`playerView`  

The player view.

## Return Value

true if the player view should automatically be miniaturized; otherwise false.

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

func playerView(AVPlayerView, failedToStartPictureInPictureWithError: any Error)

Tells the delegate that Picture in Picture playback failed to start.

func playerView(AVPlayerView, restoreUserInterfaceForPictureInPictureStopWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the user interface before Picture in Picture playback stops.

