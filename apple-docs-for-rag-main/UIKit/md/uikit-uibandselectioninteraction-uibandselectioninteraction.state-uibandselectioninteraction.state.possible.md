

- UIKit
- UIBandSelectionInteraction
- UIBandSelectionInteraction.State
-  UIBandSelectionInteraction.State.possible 

Case

# UIBandSelectionInteraction.State.possible

A state that indicates the interaction object is ready to start a new interaction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
case possible
```

## Discussion

A UIBandSelectionInteraction object in this state is waiting for events to occur that start the interaction. When an interaction concludes, the interaction returns to this state until a new interaction begins.

## See Also

### Getting the selection state

case began

A state that indicates the interaction object began a new interaction.

case selecting

A state that indicates the interaction object is tracking changes to the selection rectangle.

case ended

A state that indicates the current interaction ended.

