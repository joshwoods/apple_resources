

- AppKit
- NSSearchToolbarItem
-  searchField 

Instance Property

# searchField

The search field inside the toolbar item.

macOS 11.0+

``` source
@MainActor
var searchField: NSSearchField { get set }
```

## Discussion

When you set `searchField` to `nil`, it uses the default configuration for the toolbar item, and inherits the item’s properties and layout constraints. However, if you want to customize the search field, you’ll need to add those settings before assigning it to the toolbar item. For more information about customizing a search field, see NSSearchField.

## See Also

### Configuring a search item

var preferredWidthForSearchField: CGFloat

The preferred width for the toolbar item when it has keyboard focus.

var resignsFirstResponderWithCancel: Bool

A Boolean value that enables the cancel button in the search field to resign the first responder in addition to clearing the contents.

