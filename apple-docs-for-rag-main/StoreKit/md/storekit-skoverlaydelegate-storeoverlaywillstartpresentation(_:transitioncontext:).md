

- StoreKit
- SKOverlayDelegate
-  storeOverlayWillStartPresentation(\_:transitionContext:) 

Instance Method

# storeOverlayWillStartPresentation(\_:transitionContext:)

Indicates that the platform presents an overlay.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
optional func storeOverlayWillStartPresentation(
    _ overlay: SKOverlay,
    transitionContext: SKOverlay.TransitionContext
)
```

## Parameters 

`overlay`  

An overlay object that’s about to appear.

`transitionContext`  

A context you can use to animate changes to UI components as the overlay appears.

## Discussion

Use the `transitionContext` parameter to animate updates to the UI on the main thread. For example, make a UIImageView disappear by animating the change of its opacity to 0% as shown in the following code:

```
func storeOverlayWillStartPresentation(_ overlay: SKOverlay, transitionContext: SKOverlay.TransitionContext) {
    transitionContext.addAnimation { [self] in
        self.imageView.layer.opacity = 0
    }
}
```

## See Also

### Responding to the Overlay’s Appearance and Disappearance

func storeOverlayDidFinishPresentation(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform finished presenting an overlay.

func storeOverlayWillStartDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that the platform dismisses an overlay.

func storeOverlayDidFinishDismissal(SKOverlay, transitionContext: SKOverlay.TransitionContext)

Indicates that platform finished dismissing an overlay.

class TransitionContext

A context object you can use to animate UI changes while the platform presents or dismisses an overlay.

