

- AppKit
- NSMenuItem
-  representedObject 

Instance Property

# representedObject

The object represented by the menu item.

macOS

``` source
var representedObject: Any? { get set }
```

## Discussion

By setting a represented object for a menu item, you make an association between the menu item and that object. The represented object functions as a more specific form of tag that allows you to associate any object, not just an arbitrary integer, with the items in a menu.

## See Also

### Related Documentation

var tag: Int

The menu item’s tag.

