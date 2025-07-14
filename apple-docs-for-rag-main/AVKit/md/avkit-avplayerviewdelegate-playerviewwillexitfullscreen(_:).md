

- AVKit
- AVPlayerViewDelegate
-  playerViewWillExitFullScreen(\_:) 

Instance Method

# playerViewWillExitFullScreen(\_:)

Tells the delegate that the player view is about to exit full-screen mode.

macOS 12.0+

``` source
optional func playerViewWillExitFullScreen(_ playerView: AVPlayerView)
```

## Parameters 

`playerView`  

The player view.

## See Also

### Responding to Full Screen Events

func playerViewWillEnterFullScreen(AVPlayerView)

Tells the delegate that the player view is about to enter full-screen mode.

func playerViewDidEnterFullScreen(AVPlayerView)

Tells the delegate that the player view entered full-screen mode.

func playerViewDidExitFullScreen(AVPlayerView)

Tells the delegate that the player view exited full-screen mode.

func playerView(AVPlayerView, restoreUserInterfaceForFullScreenExitWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the app’s user interface when exiting full-screen mode.

