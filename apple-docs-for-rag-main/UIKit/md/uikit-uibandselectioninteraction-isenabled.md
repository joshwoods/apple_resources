

- UIKit
- UIBandSelectionInteraction
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that specifies whether the object is ready to detect interactions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

If the value of this property is true, the UIBandSelectionInteraction object is ready to detect pointer-based events in its owning view and initiate interactions. If the value is false, the object ignores events and doesn’t start interactions. The default value of this property is true.

## See Also

### Getting the interaction state

var initialModifierFlags: UIKeyModifierFlags

The pressed modifier keys at the start of the interaction.

var state: UIBandSelectionInteraction.State

The current state of the interaction object.

enum State

Constants that indicate whether a band selection interaction object is inactive or currently tracking an interaction.

