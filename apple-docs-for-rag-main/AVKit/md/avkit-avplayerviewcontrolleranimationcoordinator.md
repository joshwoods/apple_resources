

- AVKit
-  AVPlayerViewControllerAnimationCoordinator 

Protocol

# AVPlayerViewControllerAnimationCoordinator

A protocol that defines the methods to implement to synchronize animations with playback controls’ visibility animation.

tvOS 11.0+

``` source
protocol AVPlayerViewControllerAnimationCoordinator : NSObjectProtocol
```

## Topics

### Coordinating Animations

func addCoordinatedAnimations((() -> Void)?, completion: ((Bool) -> Void)?)

Adds animations to perform alongside the playback controls’ visibility animation.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to Transport Bar Changes

func playerViewController(AVPlayerViewController, willTransitionToVisibilityOfTransportBar: Bool, with: any AVPlayerViewControllerAnimationCoordinator)

Tells the delegate when the transport bar’s visibility is about to change.

