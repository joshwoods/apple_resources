

- AppKit
- NSLayoutManager
-  addTextContainer(\_:) 

Instance Method

# addTextContainer(\_:)

Appends the specified text container to the series of text containers where the layout manager arranges text.

macOS 10.7+

``` source
func addTextContainer(_ container: NSTextContainer)
```

## Parameters 

`container`  

The text container to append.

## Discussion

Invalidates glyphs and layout as needed, but doesn’t perform glyph generation or layout.

## See Also

### Managing the text containers

var textContainers: [NSTextContainer]

The current text containers of the layout manager.

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

func usedRect(for: NSTextContainer) -> NSRect

Returns the bounding rectangle for the glyphs in the specified text container.

