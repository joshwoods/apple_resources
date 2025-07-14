

- AppKit
- NSSearchToolbarItem
-  endSearchInteraction() 

Instance Method

# endSearchInteraction()

Ends a search interaction by giving up the first responder and adjusting the size of the search field to the available width for the toolbar item if necessary.

macOS 11.0+

``` source
@MainActor
func endSearchInteraction()
```

## Discussion

Use beginSearchInteraction() and endSearchInteraction() to programmatically control a search.

## See Also

### Controlling search interactions

func beginSearchInteraction()

Starts a search interaction and moves the keyboard focus to the search field.

