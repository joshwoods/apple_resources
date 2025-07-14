

- StoreKit
- SKOverlayDelegate
-  storeOverlayDidFinishPresentation(\_:transitionContext:) 

Instance Method

# storeOverlayDidFinishPresentation(\_:transitionContext:)

Indicates that the platform finished presenting an overlay.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
optional func storeOverlayDidFinishPresentation(
    _ overlay: SKOverlay,
    transitionContext: SKOverlay.TransitionContext
)
```

## Parameters 

`overlay`  

The overlay object that appears.

`transitionContext`  

A context you can use to animate changes to UI components after the overlay appears.

## See Also

### Responding to the Overlay’s Appearance and Disappearance

func storeOverlayWillStartPresentation(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform presents an overlay.

func storeOverlayWillStartDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform dismisses an overlay.

func storeOverlayDidFinishDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that platform finished dismissing an overlay.

class TransitionContext

A context object you can use to animate UI changes while the platform presents or dismisses an overlay.

