

- AppKit
- NSMenuDelegate
-  menuDidClose(\_:) 

Instance Method

# menuDidClose(\_:)

Invoked after a menu closed.

macOS 10.5+

``` source
@MainActor
optional func menuDidClose(_ menu: NSMenu)
```

## Parameters 

`menu`  

The menu that closed.

## Discussion

Don’t modify the structure of the menu or the menu items during this method.

## See Also

### Handling Open and Close Events

func menuWillOpen(NSMenu)

Invoked when a menu is about to open.

