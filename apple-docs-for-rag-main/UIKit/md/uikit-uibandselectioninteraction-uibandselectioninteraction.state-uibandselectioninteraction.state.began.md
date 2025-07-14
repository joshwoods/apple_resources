

- UIKit
- UIBandSelectionInteraction
- UIBandSelectionInteraction.State
-  UIBandSelectionInteraction.State.began 

Case

# UIBandSelectionInteraction.State.began

A state that indicates the interaction object began a new interaction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
case began
```

## Discussion

The interaction object enters this state once at the beginning of each interaction, and subsequently transitions to the UIBandSelectionInteraction.State.selecting or UIBandSelectionInteraction.State.ended state. When in this state, perform any one-time tasks that you need to manage your app’s state. For example, you might prepare your view to start the selection of items.

## See Also

### Getting the selection state

case possible

A state that indicates the interaction object is ready to start a new interaction.

case selecting

A state that indicates the interaction object is tracking changes to the selection rectangle.

case ended

A state that indicates the current interaction ended.

