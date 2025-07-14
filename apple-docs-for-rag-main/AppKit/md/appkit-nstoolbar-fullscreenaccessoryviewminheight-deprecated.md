

- AppKit
- NSToolbar
-  fullScreenAccessoryViewMinHeight Deprecated

Instance Property

# fullScreenAccessoryViewMinHeight

The minimum height of the toolbar’s full screen accessory view.

macOS 10.7–10.13Deprecated

``` source
@MainActor
var fullScreenAccessoryViewMinHeight: CGFloat { get set }
```

Deprecated

Use an NSTitlebarAccessoryViewController and its fullScreenMinHeight property with an NSWindow instead.

## Discussion

The fullScreenAccessoryViewMinHeight is used when the menu bar is hidden. During the reveal, the toolbar’s accessory view’s frame is interpolated between its fullScreenAccessoryViewMinHeight and fullScreenAccessoryViewMaxHeight.

If the minimum height is 0 the accessory view isn’t resized; instead a special transition is used to reveal it with the menu bar. This simplifies the accessory view’s task, because it doesn’t have to handle the case of the height being set to `0`.

To create a fixed-height accessory view, set the fullScreenAccessoryViewMaxHeight and fullScreenAccessoryViewMinHeight properties to be equal.

The default value is 0.

## See Also

### Deprecated

var centeredItemIdentifier: NSToolbarItem.Identifier?

The item to display in the center of the toolbar.

Deprecated

var fullScreenAccessoryView: NSView?

The toolbar’s full screen accessory view.

Deprecated

var fullScreenAccessoryViewMaxHeight: CGFloat

The maximum height of the toolbar’s full screen accessory view, in points.

Deprecated

var sizeMode: NSToolbar.SizeMode

The toolbar’s size mode.

Deprecated

enum SizeMode

Constants that specify toolbar display modes.

Deprecated

