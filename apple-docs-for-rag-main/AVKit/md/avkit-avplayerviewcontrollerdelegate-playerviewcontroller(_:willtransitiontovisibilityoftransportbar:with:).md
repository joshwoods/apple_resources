

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:willTransitionToVisibilityOfTransportBar:with:) 

Instance Method

# playerViewController(\_:willTransitionToVisibilityOfTransportBar:with:)

Tells the delegate when the transport bar’s visibility is about to change.

tvOS 11.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    willTransitionToVisibilityOfTransportBar visible: Bool,
    with coordinator: any AVPlayerViewControllerAnimationCoordinator
)
```

## Parameters 

`playerViewController`  

The player view controller.

`visible`  

The transport bar’s new visibility.

`coordinator`  

The animation coordinator to use to synchronize animations with the transport bar visibility.

## See Also

### Responding to Transport Bar Changes

protocol AVPlayerViewControllerAnimationCoordinator

A protocol that defines the methods to implement to synchronize animations with playback controls’ visibility animation.

