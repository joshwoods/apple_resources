

- UIKit
- UITextSelectionDisplayInteraction
-  setNeedsSelectionUpdate() 

Instance Method

# setNeedsSelectionUpdate()

Tells the system to update the selection UI to match the current selection state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func setNeedsSelectionUpdate()
```

## Mentioned in 

Adopting system selection UI in custom text views

## Discussion

When the selection state changes in your text input view, call this method to notify the system of the change. The system fetches the current selection state from your text input view and updates the system UI to match.

## See Also

### Reporting changes to the selection

func layoutManagedSubviews()

Loads the selection from the text input view and lays out the selection-related views.

