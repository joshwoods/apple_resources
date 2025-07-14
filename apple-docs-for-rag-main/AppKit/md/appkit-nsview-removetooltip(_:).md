

- AppKit
- NSView
-  removeToolTip(\_:) 

Instance Method

# removeToolTip(\_:)

Removes the tooltip identified by specified tag.

macOS

``` source
@MainActor
func removeToolTip(_ tag: NSView.ToolTipTag)
```

## Parameters 

`tag`  

An integer tag that is the value returned by a previous addToolTip(_:owner:userData:) message.

## See Also

### Providing a Tool Tip

var toolTip: String?

The text for the view’s tooltip.

func addToolTip(NSRect, owner: Any, userData: UnsafeMutableRawPointer?) -> NSView.ToolTipTag

Creates a tooltip for a defined area in the view and returns a tag that identifies the tooltip rectangle.

func removeAllToolTips()

Removes all tooltips assigned to the view.

typealias ToolTipTag

This type describes the rectangle used to identify a tooltip rectangle.

