

- AppKit
- NSViewToolTipOwner
-  view(\_:stringForToolTip:point:userData:) 

Instance Method

# view(\_:stringForToolTip:point:userData:)

Returns the tool tip string to be displayed due to the cursor pausing at location `point` within the tool tip rectangle identified by `tag` in the view `view`.

macOS

``` source
@MainActor
func view(
    _ view: NSView,
    stringForToolTip tag: NSView.ToolTipTag,
    point: NSPoint,
    userData data: UnsafeMutableRawPointer?
) -> String
```

**Required**

## Discussion

`userData` is additional information provided by the creator of the tool tip rectangle.

## See Also

### Related Documentation

Online Help

func addToolTip(NSRect, owner: Any, userData: UnsafeMutableRawPointer?) -> NSView.ToolTipTag

Creates a tooltip for a defined area in the view and returns a tag that identifies the tooltip rectangle.

