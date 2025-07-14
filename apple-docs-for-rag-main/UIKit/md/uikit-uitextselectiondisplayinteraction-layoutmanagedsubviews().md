

- UIKit
- UITextSelectionDisplayInteraction
-  layoutManagedSubviews() 

Instance Method

# layoutManagedSubviews()

Loads the selection from the text input view and lays out the selection-related views.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func layoutManagedSubviews()
```

## See Also

### Reporting changes to the selection

func setNeedsSelectionUpdate()

Tells the system to update the selection UI to match the current selection state.

