

- AppKit
- NSSearchField
-  noRecentsMenuItemTag 

Type Property

# noRecentsMenuItemTag

The menu item that describes a lack of recent search strings.

macOS

``` source
class let noRecentsMenuItemTag: Int
```

## Discussion

This item is hidden if there have been recent searches.

## See Also

### Managing Menu Templates

var searchMenuTemplate: NSMenu?

The menu object used to dynamically construct the search field’s pop-up icon menu.

class let clearRecentsMenuItemTag: Int

The menu item for clearing the current set of recent string searches in the menu.

class let recentsMenuItemTag: Int

The location of recent search strings in the “recents” menu group.

class let recentsTitleMenuItemTag: Int

The menu item that provides the title of the menu group for recent search strings.

