

- AppKit
- NSLayoutManager
-  removeTextContainer(at:) 

Instance Method

# removeTextContainer(at:)

Removes the text container at the specified index and invalidates the layout as necessary.

macOS 10.7+

``` source
func removeTextContainer(at index: Int)
```

## Parameters 

`index`  

The index of the text container to remove.

## Discussion

This method invalidates glyph information as needed.

## See Also

### Managing the text containers

var textContainers: [NSTextContainer]

The current text containers of the layout manager.

func addTextContainer(NSTextContainer)

Appends the specified text container to the series of text containers where the layout manager arranges text.

func insertTextContainer(NSTextContainer, at: Int)

Inserts a text container at the specified index in the list of text containers.

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

func usedRect(for: NSTextContainer) -> NSRect

Returns the bounding rectangle for the glyphs in the specified text container.

