

- AppKit
- NSTextAttachmentCellProtocol
-  cellBaselineOffset() 

Instance Method

# cellBaselineOffset()

Returns the text position where you draw the attachment cell’s image, relative to the current point established in the glyph layout.

macOS

``` source
nonisolated
func cellBaselineOffset() -> NSPoint
```

**Required**

## Discussion

The image should be drawn so its lower-left corner lies on this point.

## See Also

### Related Documentation

var icon: NSImage?

The icon that represents the file wrapper.

### Providing the cell metrics

func cellSize() -> NSSize

Returns the size of the attachment’s icon.

**Required**

func cellFrame(for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the frame of the cell to draw at the specified position in a text container.

**Required**

