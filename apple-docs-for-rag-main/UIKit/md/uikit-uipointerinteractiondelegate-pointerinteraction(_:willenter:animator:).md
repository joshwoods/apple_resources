

- UIKit
- UIPointerInteractionDelegate
-  pointerInteraction(\_:willEnter:animator:) 

Instance Method

# pointerInteraction(\_:willEnter:animator:)

Informs the delegate when the pointer enters a given region.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
optional func pointerInteraction(
    _ interaction: UIPointerInteraction,
    willEnter region: UIPointerRegion,
    animator: any UIPointerInteractionAnimating
)
```

## Parameters 

`interaction`  

This UIPointerInteraction.

`region`  

The UIPointerRegion that represents the entire surface of the interaction’s view.

`animator`  

The animator the framework runs when the pointer enters the region. Add animations to run them alongside the pointer’s entrance animation.

## See Also

### Handling animations for pointer regions

func pointerInteraction(UIPointerInteraction, willExit: UIPointerRegion, animator: any UIPointerInteractionAnimating)

Informs the delegate when the pointer exits a given region.

