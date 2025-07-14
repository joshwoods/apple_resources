

- AppKit
- NSToolbar
-  sizeMode Deprecated

Instance Property

# sizeMode

The toolbar’s size mode.

macOS 10.0–15.4Deprecated

``` source
@MainActor
var sizeMode: NSToolbar.SizeMode { get set }
```

Deprecated

The toolbar ignores this property.

## Discussion

If there’s no icon of the given size for a toolbar item, the toolbar item creates one by scaling an icon of another size.

## See Also

### Deprecated

var centeredItemIdentifier: NSToolbarItem.Identifier?

The item to display in the center of the toolbar.

Deprecated

var fullScreenAccessoryView: NSView?

The toolbar’s full screen accessory view.

Deprecated

var fullScreenAccessoryViewMinHeight: CGFloat

The minimum height of the toolbar’s full screen accessory view.

Deprecated

var fullScreenAccessoryViewMaxHeight: CGFloat

The maximum height of the toolbar’s full screen accessory view, in points.

Deprecated

enum SizeMode

Constants that specify toolbar display modes.

Deprecated

