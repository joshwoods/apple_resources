

- AppKit
- NSTextAttachmentCellProtocol
-  highlight(\_:withFrame:in:) 

Instance Method

# highlight(\_:withFrame:in:)

Draws the receiver’s image with optional highlighting.

macOS

``` source
@MainActor
func highlight(
    _ flag: Bool,
    withFrame cellFrame: NSRect,
    in controlView: NSView?
)
```

**Required**

## Parameters 

`flag`  

A Boolean value that indicates whether to highlight the image. Add a highlight if the value is true.

`cellFrame`  

The frame rectangle in which to draw.

`controlView`  

The view in which to draw.

## See Also

### Related Documentation

func highlight(Bool, withFrame: NSRect, in: NSView)

Redraws the receiver with the specified highlight setting.

func lockFocus()

Locks the focus on the view, so subsequent commands take effect in the view’s window and coordinate system.

Deprecated

### Drawing the cell contents

func draw(withFrame: NSRect, in: NSView?)

Draws the cell’s image in the specified rectangle of the currently focused view.

**Required**

func draw(withFrame: NSRect, in: NSView?, characterIndex: Int)

Draws the cell’s image at the specified index point in the view.

**Required**

func draw(withFrame: NSRect, in: NSView?, characterIndex: Int, layoutManager: NSLayoutManager)

Draws the cell’s image using the specified layout manager.

**Required**

