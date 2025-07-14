

- UIKit
- UIPointerInteractionDelegate
-  pointerInteraction(\_:willExit:animator:) 

Instance Method

# pointerInteraction(\_:willExit:animator:)

Informs the delegate when the pointer exits a given region.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
optional func pointerInteraction(
    _ interaction: UIPointerInteraction,
    willExit region: UIPointerRegion,
    animator: any UIPointerInteractionAnimating
)
```

## Parameters 

`interaction`  

This UIPointerInteraction.

`region`  

The UIPointerRegion that represents the entire surface of the interaction’s view.

`animator`  

The animator the framework runs when the pointer exists the region. Add animations to run them alongside the pointer’s exit animation.

## See Also

### Handling animations for pointer regions

func pointerInteraction(UIPointerInteraction, willEnter: UIPointerRegion, animator: any UIPointerInteractionAnimating)

Informs the delegate when the pointer enters a given region.

