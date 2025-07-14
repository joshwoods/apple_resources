

- UIKit
- UIBandSelectionInteraction
-  initialModifierFlags 

Instance Property

# initialModifierFlags

The pressed modifier keys at the start of the interaction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var initialModifierFlags: UIKeyModifierFlags { get }
```

## Discussion

When an interaction starts, the UIBandSelectionInteraction object places the current pressed modifier keys in this property. Use the set of modifier keys to adjust the behavior of your handler. For example, you might extend an existing selection when someone presses the Shift key.

## See Also

### Getting the interaction state

var isEnabled: Bool

A Boolean value that specifies whether the object is ready to detect interactions.

var state: UIBandSelectionInteraction.State

The current state of the interaction object.

enum State

Constants that indicate whether a band selection interaction object is inactive or currently tracking an interaction.

