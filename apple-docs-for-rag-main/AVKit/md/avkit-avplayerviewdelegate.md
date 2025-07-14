

- AVKit
-  AVPlayerViewDelegate 

Protocol

# AVPlayerViewDelegate

A protocol that defines the methods to implement to participate in the player view’s full-screen presentation life cycle.

macOS 12.0+

``` source
protocol AVPlayerViewDelegate : NSObjectProtocol
```

## Topics

### Responding to Full Screen Events

func playerViewWillEnterFullScreen(AVPlayerView)

Tells the delegate that the player view is about to enter full-screen mode.

func playerViewDidEnterFullScreen(AVPlayerView)

Tells the delegate that the player view entered full-screen mode.

func playerViewWillExitFullScreen(AVPlayerView)

Tells the delegate that the player view is about to exit full-screen mode.

func playerViewDidExitFullScreen(AVPlayerView)

Tells the delegate that the player view exited full-screen mode.

func playerView(AVPlayerView, restoreUserInterfaceForFullScreenExitWithCompletionHandler: (Bool) -> Void)

Tells the delegate to restore the app’s user interface when exiting full-screen mode.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the Delegate Object

var delegate: (any AVPlayerViewDelegate)?

The player view’s delegate object.

