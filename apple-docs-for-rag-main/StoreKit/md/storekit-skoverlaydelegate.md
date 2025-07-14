

- StoreKit
-  SKOverlayDelegate 

Protocol

# SKOverlayDelegate

Methods for responding to the overlay’s appearance, dismissal, or failure to load.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
protocol SKOverlayDelegate : NSObjectProtocol
```

## Topics

### Responding to the Overlay’s Appearance and Disappearance

func storeOverlayWillStartPresentation(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform presents an overlay.

func storeOverlayDidFinishPresentation(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform finished presenting an overlay.

func storeOverlayWillStartDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform dismisses an overlay.

func storeOverlayDidFinishDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that platform finished dismissing an overlay.

class TransitionContext

A context object you can use to animate UI changes while the platform presents or dismisses an overlay.

### Responding to Failures

func storeOverlayDidFailToLoad(SKOverlay, error: any Error)

Indicates that an overlay failed to load.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting a delegate

var delegate: (any SKOverlayDelegate)?

The overlay’s delegate.

