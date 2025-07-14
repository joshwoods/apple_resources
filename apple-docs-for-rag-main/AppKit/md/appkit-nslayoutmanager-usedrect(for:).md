

- AppKit
- NSLayoutManager
-  usedRect(for:) 

Instance Method

# usedRect(for:)

Returns the bounding rectangle for the glyphs in the specified text container.

macOS 10.7+

``` source
func usedRect(for container: NSTextContainer) -> NSRect
```

## Discussion

Returns the text container’s currently used area, which determines the size that the view would need to be in order to display all the glyphs that are currently laid out in the container. This causes neither glyph generation nor layout.

Used rectangles are always in container coordinates.

## See Also

### Managing the text containers

var textContainers: [NSTextContainer]

The current text containers of the layout manager.

func addTextContainer(NSTextContainer)

Appends the specified text container to the series of text containers where the layout manager arranges text.

func insertTextContainer(NSTextContainer, at: Int)

Inserts a text container at the specified index in the list of text containers.

func removeTextContainer(at: Int)

Removes the text container at the specified index and invalidates the layout as necessary.

func setTextContainer(NSTextContainer, forGlyphRange: NSRange)

Associates a text container with the specified range of glyphs.

func textContainerChangedGeometry(NSTextContainer)

Invalidates the layout information, and possibly glyphs, for the specified text container and all subsequent text container objects.

func textContainerChangedTextView(NSTextContainer)

Updates the information necessary to manage text view objects for the specified text container.

func textContainer(forGlyphAt: Int, effectiveRange: NSRangePointer?) -> NSTextContainer?

Returns the text container that manages the layout for the specified glyph, causing layout to happen as necessary.

func textContainer(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> NSTextContainer?

Returns the text container that manages the layout for the specified glyph.

