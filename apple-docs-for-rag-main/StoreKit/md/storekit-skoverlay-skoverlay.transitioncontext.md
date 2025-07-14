

- StoreKit
- SKOverlay
-  SKOverlay.TransitionContext 

Class

# SKOverlay.TransitionContext

A context object you can use to animate UI changes while the platform presents or dismisses an overlay.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class TransitionContext
```

## Overview

For more information on animating UI changes while the system presents or dismisses an overlay, see storeOverlayWillStartPresentation(_:transitionContext:) and storeOverlayWillStartDismissal(_:transitionContext:).

## Topics

### Adding an Animation

func addAnimation(() -> Void)

Adds a closure you can use to animate view properties.

var startFrame: CGRect

The size and location of the overlay before the transition.

var endFrame: CGRect

The size and location of the overlay at the end of the transition.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Responding to the Overlay’s Appearance and Disappearance

func storeOverlayWillStartPresentation(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform presents an overlay.

func storeOverlayDidFinishPresentation(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform finished presenting an overlay.

func storeOverlayWillStartDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform dismisses an overlay.

func storeOverlayDidFinishDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that platform finished dismissing an overlay.

