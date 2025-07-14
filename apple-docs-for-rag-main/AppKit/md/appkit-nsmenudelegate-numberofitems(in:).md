

- AppKit
- NSMenuDelegate
-  numberOfItems(in:) 

Instance Method

# numberOfItems(in:)

Invoked when a menu is about to be displayed at the start of a tracking session so the delegate can specify the number of items in the menu.

macOS

``` source
@MainActor
optional func numberOfItems(in menu: NSMenu) -> Int
```

## Parameters 

`menu`  

The menu object about to be displayed.

## Return Value

The number of menu items in the menu.

## Discussion

If you return a positive value, the menu is resized by either removing or adding items. Newly created items are blank. After the menu is resized, your menu(_:update:at:shouldCancel:) method is called for each item. If you return a negative value, the number of items is left unchanged and menu(_:update:at:shouldCancel:) is not called. If you can populate the menu quickly, you can implement menuNeedsUpdate(_:) instead of numberOfItems(in:) and menu(_:update:at:shouldCancel:).

## See Also

### Handling Tracking

func menuNeedsUpdate(NSMenu)

Invoked when a menu is about to be displayed at the start of a tracking session.

