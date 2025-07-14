

- AppKit
- NSSearchField
-  searchMenuTemplate 

Instance Property

# searchMenuTemplate

The menu object used to dynamically construct the search field’s pop-up icon menu.

macOS 10.10+

``` source
@MainActor
var searchMenuTemplate: NSMenu? { get set }
```

## See Also

### Related Documentation

Search Fields

### Managing Menu Templates

class let clearRecentsMenuItemTag: Int

The menu item for clearing the current set of recent string searches in the menu.

class let noRecentsMenuItemTag: Int

The menu item that describes a lack of recent search strings.

class let recentsMenuItemTag: Int

The location of recent search strings in the “recents” menu group.

class let recentsTitleMenuItemTag: Int

The menu item that provides the title of the menu group for recent search strings.

