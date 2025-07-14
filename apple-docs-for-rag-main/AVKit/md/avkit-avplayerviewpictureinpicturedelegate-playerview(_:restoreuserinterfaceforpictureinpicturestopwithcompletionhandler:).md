

- AVKit
- AVPlayerViewPictureInPictureDelegate
-  playerView(\_:restoreUserInterfaceForPictureInPictureStopWithCompletionHandler:) 

Instance Method

# playerView(\_:restoreUserInterfaceForPictureInPictureStopWithCompletionHandler:)

Tells the delegate to restore the user interface before Picture in Picture playback stops.

macOS 10.15+

``` source
optional func playerView(
    _ playerView: AVPlayerView,
    restoreUserInterfaceForPictureInPictureStopWithCompletionHandler completionHandler: @escaping (Bool) -> Void
)
```

``` source
optional func playerViewRestoreUserInterfaceForPictureInPictureStop(_ playerView: AVPlayerView) async -> Bool
```

## Parameters 

`playerView`  

The player view.

`completionHandler`  

The completion handler to call after you’ve restored the user interface.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func playerViewRestoreUserInterfaceForPictureInPictureStop(_ playerView: AVPlayerView) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

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

func playerViewShouldAutomaticallyDismissAtPicture(inPictureStart: AVPlayerView) -> Bool

Asks the delegate if the player view should miniaturize when Picture in Picture starts.

