

- StoreKit
- SKOverlayDelegate
-  storeOverlayDidFinishDismissal(\_:transitionContext:) 

Instance Method

# storeOverlayDidFinishDismissal(\_:transitionContext:)

Indicates that platform finished dismissing an overlay.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
optional func storeOverlayDidFinishDismissal(
    _ overlay: SKOverlay,
    transitionContext: SKOverlay.TransitionContext
)
```

## Parameters 

`overlay`  

An app banner object that disappeared.

`transitionContext`  

The context you can use to animate changes to UI components when the overlay disappears.

## See Also

### Responding to the Overlay’s Appearance and Disappearance

func storeOverlayWillStartPresentation(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform presents an overlay.

func storeOverlayDidFinishPresentation(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform finished presenting an overlay.

func storeOverlayWillStartDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform dismisses an overlay.

class TransitionContext

A context object you can use to animate UI changes while the platform presents or dismisses an overlay.

