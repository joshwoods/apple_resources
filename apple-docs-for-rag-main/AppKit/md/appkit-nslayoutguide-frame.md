

- AppKit
- NSLayoutGuide
-  frame 

Instance Property

# frame

The layout guide’s frame in its owning view’s coordinate system.

macOS 10.11+

``` source
var frame: NSRect { get }
```

## Discussion

The layout guide defines a rectangular space in its owning view’s coordinate system. This property contains a valid CGRect value by the time its owning view’s layout() method is called.

## See Also

### Related Documentation

func layout()

Perform layout in concert with the constraint-based layout system.

### Working With Layout Guides

var identifier: NSUserInterfaceItemIdentifier

A string used to identify the layout guide.

var owningView: NSView?

The view that owns this layout guide.

