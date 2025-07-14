

- UIKit
- UIPointerInteractionDelegate
-  pointerInteraction(\_:styleFor:) 

Instance Method

# pointerInteraction(\_:styleFor:)

Asks the delegate for a pointer style after an interaction receives a new region.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
optional func pointerInteraction(
    _ interaction: UIPointerInteraction,
    styleFor region: UIPointerRegion
) -> UIPointerStyle?
```

## Parameters 

`interaction`  

This UIPointerInteraction.

`region`  

The UIPointerRegion that represents the entire surface of the interaction’s view.

## Return Value

A `UIPointerStyle` describing the desired hover effect or pointer appearance for the given `UIPointerRegion`.

## See Also

### Defining pointer styles for regions

func pointerInteraction(UIPointerInteraction, regionFor: UIPointerRegionRequest, defaultRegion: UIPointerRegion) -> UIPointerRegion?

Asks the delegate for a region as the pointer moves within the interaction’s view.

