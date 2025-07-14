

- AppKit
- NSView
-  removeAllToolTips() 

Instance Method

# removeAllToolTips()

Removes all tooltips assigned to the view.

macOS

``` source
@MainActor
func removeAllToolTips()
```

## Discussion

This method operates on tooltips created using either addToolTip(_:owner:userData:) or set using the toolTip property.

## See Also

### Providing a Tool Tip

var toolTip: String?

The text for the view’s tooltip.

func addToolTip(NSRect, owner: Any, userData: UnsafeMutableRawPointer?) -> NSView.ToolTipTag

Creates a tooltip for a defined area in the view and returns a tag that identifies the tooltip rectangle.

func removeToolTip(NSView.ToolTipTag)

Removes the tooltip identified by specified tag.

typealias ToolTipTag

This type describes the rectangle used to identify a tooltip rectangle.

