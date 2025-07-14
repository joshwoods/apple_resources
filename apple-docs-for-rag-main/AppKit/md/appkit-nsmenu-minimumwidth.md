

- AppKit
- NSMenu
-  minimumWidth 

Instance Property

# minimumWidth

The minimum width of the menu in screen coordinates.

macOS 10.6+

``` source
var minimumWidth: CGFloat { get set }
```

## Discussion

This property contains a value of type `CGFloat`, indicating the minimum width of the menu in screen coordinates.

The menu will not draw smaller than its minimum width, but may draw larger if it needs more space. The default value for this property is `0`.

## See Also

### Configuring Menu Size

var size: NSSize

The size of the menu in screen coordinates

