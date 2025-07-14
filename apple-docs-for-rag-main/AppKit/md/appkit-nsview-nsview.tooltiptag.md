

- AppKit
- NSView
-  NSView.ToolTipTag 

Type Alias

# NSView.ToolTipTag

This type describes the rectangle used to identify a tooltip rectangle.

macOS

``` source
typealias ToolTipTag = Int
```

## Discussion

If the value of this type is 0, it is invalid. See the methods addToolTip(_:owner:userData:) andremoveToolTip(_:).

## See Also

### Providing a Tool Tip

var toolTip: String?

The text for the view’s tooltip.

func addToolTip(NSRect, owner: Any, userData: UnsafeMutableRawPointer?) -> NSView.ToolTipTag

Creates a tooltip for a defined area in the view and returns a tag that identifies the tooltip rectangle.

func removeAllToolTips()

Removes all tooltips assigned to the view.

func removeToolTip(NSView.ToolTipTag)

Removes the tooltip identified by specified tag.

