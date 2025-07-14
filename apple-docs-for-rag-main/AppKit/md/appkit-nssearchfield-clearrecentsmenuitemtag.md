

- AppKit
- NSSearchField
-  clearRecentsMenuItemTag 

Type Property

# clearRecentsMenuItemTag

The menu item for clearing the current set of recent string searches in the menu.

macOS

``` source
class let clearRecentsMenuItemTag: Int
```

## Discussion

This item is hidden if there are no recent strings.

## See Also

### Managing Menu Templates

var searchMenuTemplate: NSMenu?

The menu object used to dynamically construct the search field’s pop-up icon menu.

class let noRecentsMenuItemTag: Int

The menu item that describes a lack of recent search strings.

class let recentsMenuItemTag: Int

The location of recent search strings in the “recents” menu group.

class let recentsTitleMenuItemTag: Int

The menu item that provides the title of the menu group for recent search strings.

