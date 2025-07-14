

- AppKit
- NSMenu
- NSMenu.SelectionMode
-  NSMenu.SelectionMode.selectAny 

Case

# NSMenu.SelectionMode.selectAny

A selection mode where someone can select multiple items in the menu.

macOS 14.0+

``` source
case selectAny
```

## Discussion

A change in selection doesn’t automatically deselect any previously selected item in the same selection group.

## See Also

### Defining the selection mode

case automatic

A selection mode where the menu determines the appropriate selection mode based on the context and its constants.

case selectOne

A selection mode where someone can select at most one menu item in the same selection group at the same time.

