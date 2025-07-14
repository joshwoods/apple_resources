

- AppKit
- NSTextAttachmentCellProtocol
-  draw(withFrame:in:) 

Instance Method

# draw(withFrame:in:)

Draws the cell’s image in the specified rectangle of the currently focused view.

macOS

``` source
@MainActor
func draw(
    withFrame cellFrame: NSRect,
    in controlView: NSView?
)
```

**Required**

## Parameters 

`cellFrame`  

The frame rectangle in which to draw.

`controlView`  

The view in which to draw.

## See Also

### Related Documentation

func draw(withFrame: NSRect, in: NSView)

Draws the receiver’s border and then draws the interior of the cell.

Text Attachment Programming Topics

func lockFocus()

Locks the focus on the view, so subsequent commands take effect in the view’s window and coordinate system.

Deprecated

### Drawing the cell contents

func draw(withFrame: NSRect, in: NSView?, characterIndex: Int)

Draws the cell’s image at the specified index point in the view.

**Required**

func draw(withFrame: NSRect, in: NSView?, characterIndex: Int, layoutManager: NSLayoutManager)

Draws the cell’s image using the specified layout manager.

**Required**

func highlight(Bool, withFrame: NSRect, in: NSView?)

Draws the receiver’s image with optional highlighting.

**Required**

