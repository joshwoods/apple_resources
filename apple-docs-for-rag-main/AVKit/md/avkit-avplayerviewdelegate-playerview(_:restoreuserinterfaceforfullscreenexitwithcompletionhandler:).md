

- AVKit
- AVPlayerViewDelegate
-  playerView(\_:restoreUserInterfaceForFullScreenExitWithCompletionHandler:) 

Instance Method

# playerView(\_:restoreUserInterfaceForFullScreenExitWithCompletionHandler:)

Tells the delegate to restore the app’s user interface when exiting full-screen mode.

macOS 12.0+

``` source
optional func playerView(
    _ playerView: AVPlayerView,
    restoreUserInterfaceForFullScreenExitWithCompletionHandler completionHandler: @escaping (Bool) -> Void
)
```

``` source
optional func playerViewRestoreUserInterfaceForFullScreenExit(_ playerView: AVPlayerView) async -> Bool
```

## Parameters 

`playerView`  

The player view.

`completionHandler`  

You must call the completion handler with a value of true to allow the system to finish restoring your app’s user interface.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
optional func playerViewRestoreUserInterfaceForFullScreenExit(_ playerView: AVPlayerView) async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Responding to Full Screen Events

func playerViewWillEnterFullScreen(AVPlayerView)

Tells the delegate that the player view is about to enter full-screen mode.

func playerViewDidEnterFullScreen(AVPlayerView)

Tells the delegate that the player view entered full-screen mode.

func playerViewWillExitFullScreen(AVPlayerView)

Tells the delegate that the player view is about to exit full-screen mode.

func playerViewDidExitFullScreen(AVPlayerView)

Tells the delegate that the player view exited full-screen mode.

