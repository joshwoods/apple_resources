

- AppKit
- NSTextAttachmentCellProtocol
-  cellSize() 

Instance Method

# cellSize()

Returns the size of the attachment’s icon.

macOS

``` source
nonisolated
func cellSize() -> NSSize
```

**Required**

## See Also

### Related Documentation

var icon: NSImage?

The icon that represents the file wrapper.

var fileWrapper: FileWrapper?

The text attachment’s file wrapper.

### Providing the cell metrics

func cellBaselineOffset() -> NSPoint

Returns the text position where you draw the attachment cell’s image, relative to the current point established in the glyph layout.

**Required**

func cellFrame(for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the frame of the cell to draw at the specified position in a text container.

**Required**

