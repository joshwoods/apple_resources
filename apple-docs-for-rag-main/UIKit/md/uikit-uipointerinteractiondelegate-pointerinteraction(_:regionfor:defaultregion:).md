

- UIKit
- UIPointerInteractionDelegate
-  pointerInteraction(\_:regionFor:defaultRegion:) 

Instance Method

# pointerInteraction(\_:regionFor:defaultRegion:)

Asks the delegate for a region as the pointer moves within the interaction’s view.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
optional func pointerInteraction(
    _ interaction: UIPointerInteraction,
    regionFor request: UIPointerRegionRequest,
    defaultRegion: UIPointerRegion
) -> UIPointerRegion?
```

## Parameters 

`interaction`  

This UIPointerInteraction.

`request`  

The UIPointerRegionRequest that describes the pointer’s location in the interaction’s view.

`defaultRegion`  

The UIPointerRegion that represents the entire surface of the interaction’s view.

## Return Value

A `UIPointerRegion` in which to apply a pointer style. Return `nil` to indicate that this interaction typically doesn’t customize the pointer for the current location.

## See Also

### Defining pointer styles for regions

func pointerInteraction(UIPointerInteraction, styleFor: UIPointerRegion) -> UIPointerStyle?

Asks the delegate for a pointer style after an interaction receives a new region.

