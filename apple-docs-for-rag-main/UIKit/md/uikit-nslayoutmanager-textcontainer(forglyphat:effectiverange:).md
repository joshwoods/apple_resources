

- UIKit
- NSLayoutManager
-  textContainer(forGlyphAt:effectiveRange:) 

Instance Method

# textContainer(forGlyphAt:effectiveRange:)

Returns the text container that manages the layout for the specified glyph, causing layout to happen as necessary.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func textContainer(
    forGlyphAt glyphIndex: Int,
    effectiveRange effectiveGlyphRange: NSRangePointer?
) -> NSTextContainer?
```

## Parameters 

`glyphIndex`  

Index of a glyph in the returned container.

`effectiveGlyphRange`  

If not `NULL`, on output, points to the whole range of glyphs that are in the returned container.

## Return Value

The text container in which the glyph at `glyphIndex` is laid out.

## Discussion

This method causes glyph generation and layout for the line fragment containing the specified glyph, or if noncontiguous layout is not enabled, up to and including that line fragment. If noncontiguous layout is not enabled and `effectiveGlyphRange` is not `NULL`, this method additionally causes glyph generation and layout for the entire text container containing the specified glyph.

Overriding this method is not recommended. Any changes to the returned glyph range should be done at the typesetter level.

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

func textContainerChangedTextView(_ container: NSTextContainer)

Updates the information necessary to manage text view objects for the specified text container.

func textContainer(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> NSTextContainer?

Returns the text container that manages the layout for the specified glyph.

func usedRect(for: NSTextContainer) -> CGRect

Returns the bounding rectangle for the glyphs in the specified text container.

