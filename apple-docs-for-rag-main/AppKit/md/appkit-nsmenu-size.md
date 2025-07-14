

- AppKit
- NSMenu
-  size 

Instance Property

# size

The size of the menu in screen coordinates

macOS 10.6+

``` source
var size: NSSize { get }
```

## Discussion

This property contains a value of type `NSSize`, indicating the size of the menu in screen coordinates.

The menu may draw at a smaller size when shown, depending on its positioning and display configuration.

## See Also

### Configuring Menu Size

var minimumWidth: CGFloat

The minimum width of the menu in screen coordinates.

