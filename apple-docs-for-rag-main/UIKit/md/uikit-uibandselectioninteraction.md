

- UIKit
-  UIBandSelectionInteraction 

Class

# UIBandSelectionInteraction

An object that tracks the selection of multiple items using pointer-based input.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class UIBandSelectionInteraction
```

## Overview

Attach a UIBandSelectionInteraction object to a custom view that contains one or more selectable items. On devices with pointer-based input, such as an iPad with a Magic Keyboard, this interaction object displays a visible selection rectangle over the view when someone clicks and drags on it. As the pointer moves, the selection rectangle expands or contracts to match. Use your interaction object’s handler to select items based on the current selection rectangle.

You create a band selection interaction object and add it to a view that contains one or more selectable items. When you create the interaction object, specify a handler to process changes to the selection rectangle. In the example, the custom view defines an `itemsInRect` method to get the items that intersect the selection rectangle. It also defines custom methods to modify the selection and commit the changes. If someone presses the Shift key at the start of the interaction, the code extends the current selection instead of replacing it.

```
// Create a UIBandSelectionInteraction object.
let bandSelectionInteraction = UIBandSelectionInteraction { [weak self] interaction in
    guard let strongSelf = self else { return }

    switch interaction.state {
    case .began:
        // Prepare the view to handle selection changes.
        strongSelf.selectionSession.begin()
    case .selecting:
        // Get the custom view items that intersect the selection rectangle.
        let newItems = strongSelf.itemsInRect(interaction.selectionRect)

        if interaction.initialModifierFlags == .shift {
            // If Shift is held, extend the view's current selection...
            strongSelf.selectionSession.append(newItems)
        } else {
            // ...otherwise, replace the view's selection with the new items.
            strongSelf.selectionSession.setSelection(newItems)
        }
    case .ended:
        // When the interaction ends, commit the selection changes.
        strongSelf.selectionSession.commit()
    }
}

// Add the interaction object to the view.
view.addInteraction(bandSelectionInteraction)
```

Note

You don’t need to add this interaction object to a collection view to handle the selection of items. UICollectionView already supports its own multiple selection interface. For a list of methods you use to manage selections in a collection view, see UICollectionViewDelegate.

## Topics

### Creating a band selection interaction

init((UIBandSelectionInteraction) -> Void)

Creates a new band selection interaction object with the provided handler code.

### Getting the selection rectangle

var selectionRect: CGRect?

The selection rectangle for an in-progress interaction.

### Getting the interaction state

var isEnabled: Bool

A Boolean value that specifies whether the object is ready to detect interactions.

var initialModifierFlags: UIKeyModifierFlags

The pressed modifier keys at the start of the interaction.

var state: UIBandSelectionInteraction.State

The current state of the interaction object.

enum State

Constants that indicate whether a band selection interaction object is inactive or currently tracking an interaction.

### Starting the interaction

var shouldBeginHandler: ((UIBandSelectionInteraction, CGPoint) -> Bool)?

The handler that determines whether to start a band selection interaction.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIInteraction

## See Also

### Band selection

enum State

Constants that indicate whether a band selection interaction object is inactive or currently tracking an interaction.

