

- AppKit
- NSMenuDelegate
-  menuWillOpen(\_:) 

Instance Method

# menuWillOpen(\_:)

Invoked when a menu is about to open.

macOS 10.5+

``` source
@MainActor
optional func menuWillOpen(_ menu: NSMenu)
```

## Parameters 

`menu`  

The menu that is about to open.

## Discussion

Don’t modify the structure of the menu or the menu items during this method.

## See Also

### Handling Open and Close Events

func menuDidClose(NSMenu)

Invoked after a menu closed.

