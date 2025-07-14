

- AppKit
- NSSearchToolbarItem
-  preferredWidthForSearchField 

Instance Property

# preferredWidthForSearchField

The preferred width for the toolbar item when it has keyboard focus.

macOS 11.0+

``` source
@MainActor
var preferredWidthForSearchField: CGFloat { get set }
```

## See Also

### Configuring a search item

var resignsFirstResponderWithCancel: Bool

A Boolean value that enables the cancel button in the search field to resign the first responder in addition to clearing the contents.

var searchField: NSSearchField

The search field inside the toolbar item.

