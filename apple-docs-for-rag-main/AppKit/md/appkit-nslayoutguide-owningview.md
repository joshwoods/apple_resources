

- AppKit
- NSLayoutGuide
-  owningView 

Instance Property

# owningView

The view that owns this layout guide.

macOS 10.11+

``` source
weak var owningView: NSView? { get set }
```

## Discussion

By default, this property is `nil`. To participate in Auto Layout, the layout guide must be added to a view by calling its addLayoutGuide(_:) method. Do not modify this property directly. Instead, use the view’s addLayoutGuide(_:) and removeLayoutGuide(_:) methods, which update this property as necessary.

## See Also

### Working With Layout Guides

var identifier: NSUserInterfaceItemIdentifier

A string used to identify the layout guide.

var frame: NSRect

The layout guide’s frame in its owning view’s coordinate system.

