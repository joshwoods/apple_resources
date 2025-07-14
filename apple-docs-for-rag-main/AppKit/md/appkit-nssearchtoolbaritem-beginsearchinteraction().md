

- AppKit
- NSSearchToolbarItem
-  beginSearchInteraction() 

Instance Method

# beginSearchInteraction()

Starts a search interaction and moves the keyboard focus to the search field.

macOS 11.0+

``` source
@MainActor
func beginSearchInteraction()
```

## Discussion

If the system displays a compressed search field, starting the search interaction expands the field to the width stored in the preferredWidthForSearchField property and moves the keyboard focus into the search field. Use beginSearchInteraction() and endSearchInteraction() to programmatically control a search.

## See Also

### Controlling search interactions

func endSearchInteraction()

Ends a search interaction by giving up the first responder and adjusting the size of the search field to the available width for the toolbar item if necessary.

