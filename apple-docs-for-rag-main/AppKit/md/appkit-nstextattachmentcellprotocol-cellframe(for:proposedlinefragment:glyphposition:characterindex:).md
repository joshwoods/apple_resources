

- AppKit
- NSTextAttachmentCellProtocol
-  cellFrame(for:proposedLineFragment:glyphPosition:characterIndex:) 

Instance Method

# cellFrame(for:proposedLineFragment:glyphPosition:characterIndex:)

Returns the frame of the cell to draw at the specified position in a text container.

macOS 10.0+

``` source
nonisolated
func cellFrame(
    for textContainer: NSTextContainer,
    proposedLineFragment lineFrag: NSRect,
    glyphPosition position: NSPoint,
    characterIndex charIndex: Int
) -> NSRect
```

**Required**

## Parameters 

`textContainer`  

The text container that contains the glyph.

`lineFrag`  

The line fragment that contains the glyph.

`position`  

The position of the glyph in the text container.

`charIndex`  

The index of the character.

## Discussion

The proposed line fragment is specified by `lineFrag`.

## See Also

### Providing the cell metrics

func cellSize() -> NSSize

Returns the size of the attachment’s icon.

**Required**

func cellBaselineOffset() -> NSPoint

Returns the text position where you draw the attachment cell’s image, relative to the current point established in the glyph layout.

**Required**

