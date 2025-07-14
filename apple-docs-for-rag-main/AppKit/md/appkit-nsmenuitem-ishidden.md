

- AppKit
- NSMenuItem
-  isHidden 

Instance Property

# isHidden

A Boolean value that indicates whether the menu item is hidden.

macOS 10.5+

``` source
var isHidden: Bool { get set }
```

## Discussion

Hidden menu items (or items with a hidden superitem) do not appear in a menu and do not participate in command key matching.

## See Also

### Managing hidden status

var isHiddenOrHasHiddenAncestor: Bool

A Boolean value that indicates whether the menu item or any of its superitems is hidden.

