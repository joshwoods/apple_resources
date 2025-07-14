

- AppKit
- NSMenu
- NSMenu.SelectionMode
-  NSMenu.SelectionMode.selectOne 

Case

# NSMenu.SelectionMode.selectOne

A selection mode where someone can select at most one menu item in the same selection group at the same time.

macOS 14.0+

``` source
case selectOne
```

## Discussion

A change in selection deselects any previously selected item.

## See Also

### Defining the selection mode

case automatic

A selection mode where the menu determines the appropriate selection mode based on the context and its constants.

case selectAny

A selection mode where someone can select multiple items in the menu.

