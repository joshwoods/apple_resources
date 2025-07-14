

- AppKit
- NSView
-  addToolTip(\_:owner:userData:) 

Instance Method

# addToolTip(\_:owner:userData:)

Creates a tooltip for a defined area in the view and returns a tag that identifies the tooltip rectangle.

macOS

``` source
@MainActor
func addToolTip(
    _ rect: NSRect,
    owner: Any,
    userData data: UnsafeMutableRawPointer?
) -> NSView.ToolTipTag
```

## Parameters 

`rect`  

A rectangle defining the region of the view to associate the tooltip with.

`owner`  

An object from which to obtain the tooltip string. The object should either implement view:stringForToolTip:point:userData:, or return a suitable string from its description method. It can therefore simply be an NSString object.

Important

The view maintains a weak reference to `owner`. You’re responsible for ensuring that `owner` remains valid for as long as it may be needed.

`data`  

Any additional information you want to pass to view:stringForToolTip:point:userData:; it isn’t used if `owner` doesn’t implement this method.

## Return Value

An integer tag identifying the tooltip; you can use this tag to remove the tooltip.

## Discussion

The tooltip string is obtained dynamically from `owner` by invoking either the `NSToolTipOwner` informal protocol method view:stringForToolTip:point:userData:, if implemented, or the NSObjectProtocol protocol method description.

## See Also

### Providing a Tool Tip

var toolTip: String?

The text for the view’s tooltip.

func removeAllToolTips()

Removes all tooltips assigned to the view.

func removeToolTip(NSView.ToolTipTag)

Removes the tooltip identified by specified tag.

typealias ToolTipTag

This type describes the rectangle used to identify a tooltip rectangle.

