

- UIKit
- UIBandSelectionInteraction
-  state 

Instance Property

# state

The current state of the interaction object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var state: UIBandSelectionInteraction.State { get }
```

## Discussion

Use the current state to determine what actions to take in your handler. For example, when an interaction object is in the selecting state, you might highlight items in your view that are inside the current selection rectangle.

## See Also

### Getting the interaction state

var isEnabled: Bool

A Boolean value that specifies whether the object is ready to detect interactions.

var initialModifierFlags: UIKeyModifierFlags

The pressed modifier keys at the start of the interaction.

enum State

Constants that indicate whether a band selection interaction object is inactive or currently tracking an interaction.

