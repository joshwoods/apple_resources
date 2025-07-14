

- AppKit
- NSSearchToolbarItem
-  resignsFirstResponderWithCancel 

Instance Property

# resignsFirstResponderWithCancel

A Boolean value that enables the cancel button in the search field to resign the first responder in addition to clearing the contents.

macOS 11.0+

``` source
@MainActor
var resignsFirstResponderWithCancel: Bool { get set }
```

## Discussion

The default value is `true`. If set to `false`, the cancel button only clears the contents of the search field.

## See Also

### Configuring a search item

var preferredWidthForSearchField: CGFloat

The preferred width for the toolbar item when it has keyboard focus.

var searchField: NSSearchField

The search field inside the toolbar item.

