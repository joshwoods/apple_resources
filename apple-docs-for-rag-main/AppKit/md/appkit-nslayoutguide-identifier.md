

- AppKit
- NSLayoutGuide
-  identifier 

Instance Property

# identifier

A string used to identify the layout guide.

macOS 10.11+

``` source
var identifier: NSUserInterfaceItemIdentifier { get set }
```

## Discussion

By default, the `identifier` property is `nil`. You can assign a string to help identify this guide. This string appears as part of the guide’s description when the guide is printed to the console. You can also use the identifier to find a particular layout guide from among the guides owned by a view.

Identifiers starting with “NS” or “UI” are reserved by the system. The system may assign these identifiers to the guides it creates.

## See Also

### Working With Layout Guides

var frame: NSRect

The layout guide’s frame in its owning view’s coordinate system.

var owningView: NSView?

The view that owns this layout guide.

