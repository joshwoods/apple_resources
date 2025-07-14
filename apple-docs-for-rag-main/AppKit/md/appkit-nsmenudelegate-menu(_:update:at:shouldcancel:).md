

- AppKit
- NSMenuDelegate
-  menu(\_:update:at:shouldCancel:) 

Instance Method

# menu(\_:update:at:shouldCancel:)

Invoked to let the delegate update a menu item before it is displayed.

macOS

``` source
@MainActor
optional func menu(
    _ menu: NSMenu,
    update item: NSMenuItem,
    at index: Int,
    shouldCancel: Bool
) -> Bool
```

## Parameters 

`menu`  

The menu object that owns `item`.

`item`  

The menu-item object that may be updated.

`index`  

The integer index of the menu item.

`shouldCancel`  

Set to true if, due to some user action, the menu no longer needs to be displayed before all the menu items have been updated. You can ignore this flag, return true, and continue; or you can save your work (to save time the next time your delegate is called) and return false to stop the updating.

## Return Value

true to continue the process. If you return false, your menu(_:update:at:shouldCancel:) is not called again. In that case, it’s your responsibility to trim any extra items from the menu.

## Discussion

If your numberOfItems(in:) delegate method returns a positive value, then your menu(_:update:at:shouldCancel:) method is called for each item in the menu. You can then update the menu title, image, and so forth for each menu item.

## See Also

### Updating Menu Layout

func confinementRect(for: NSMenu, on: NSScreen?) -> NSRect

Invoked to allow the delegate to specify a display location for the menu.

