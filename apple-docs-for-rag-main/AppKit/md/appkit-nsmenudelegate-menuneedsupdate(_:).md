

- AppKit
- NSMenuDelegate
-  menuNeedsUpdate(\_:) 

Instance Method

# menuNeedsUpdate(\_:)

Invoked when a menu is about to be displayed at the start of a tracking session.

macOS

``` source
@MainActor
optional func menuNeedsUpdate(_ menu: NSMenu)
```

## Parameters 

`menu`  

The menu object that is about to be displayed.

## Discussion

Using this method, the delegate can change the menu by adding, removing, or modifying menu items. If populating the menu will take a long time, implement numberOfItems(in:) and menu(_:update:at:shouldCancel:) instead.

Menu item validation occurs after this method is called. If the menu is updated because the user pressed a command key, only the menu item with the matching command key is validated; if the menu is updated because the user opened it, then every menu item is validated.

## See Also

### Handling Tracking

func numberOfItems(in: NSMenu) -> Int

Invoked when a menu is about to be displayed at the start of a tracking session so the delegate can specify the number of items in the menu.

