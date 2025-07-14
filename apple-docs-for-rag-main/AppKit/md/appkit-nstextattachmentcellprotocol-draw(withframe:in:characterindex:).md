

- AppKit
- NSTextAttachmentCellProtocol
-  draw(withFrame:in:characterIndex:) 

Instance Method

# draw(withFrame:in:characterIndex:)

Draws the cell’s image at the specified index point in the view.

macOS

``` source
@MainActor
func draw(
    withFrame cellFrame: NSRect,
    in controlView: NSView?,
    characterIndex charIndex: Int
)
```

**Required**

## Parameters 

`cellFrame`  

The frame rectangle in which to draw.

`controlView`  

The view in which to draw.

`charIndex`  

The index of the attachment character within the text.

## See Also

### Drawing the cell contents

func draw(withFrame: NSRect, in: NSView?)

Draws the cell’s image in the specified rectangle of the currently focused view.

**Required**

func draw(withFrame: NSRect, in: NSView?, characterIndex: Int, layoutManager: NSLayoutManager)

Draws the cell’s image using the specified layout manager.

**Required**

func highlight(Bool, withFrame: NSRect, in: NSView?)

Draws the receiver’s image with optional highlighting.

**Required**

