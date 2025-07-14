

- UIKit
- NSLayoutManager
-  insertTextContainer(\_:at:) 

Instance Method

# insertTextContainer(\_:at:)

Inserts a text container at the specified index in the list of text containers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func insertTextContainer(
    _ container: NSTextContainer,
    at index: Int
)
```

## Parameters 

`container`  

The text container to insert.

`index`  

The index in the series of text containers at which to insert `aTextContainer`.

## Discussion

This method invalidates layout for all subsequent `NSTextContainer` objects, and invalidates glyph information as needed.

## See Also

### Managing the text containers

var textContainers: [NSTextContainer]

The current text containers of the layout manager.

func addTextContainer(NSTextContainer)

Appends the specified text container to the series of text containers where the layout manager arranges text.

func removeTextContainer(at: Int)

Removes the text container at the specified index and invalidates the layout as necessary.

func setTextContainer(NSTextContainer, forGlyphRange: NSRange)

Associates a text container with the specified range of glyphs.

func textContainerChangedGeometry(NSTextContainer)

Invalidates the layout information, and possibly glyphs, for the specified text container and all subsequent text container objects.

func textContainerChangedTextView(_ container: NSTextContainer)

Updates the information necessary to manage text view objects for the specified text container.

func textContainer(forGlyphAt: Int, effectiveRange: NSRangePointer?) -> NSTextContainer?

Returns the text container that manages the layout for the specified glyph, causing layout to happen as necessary.

func textContainer(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> NSTextContainer?

Returns the text container that manages the layout for the specified glyph.

func usedRect(for: NSTextContainer) -> CGRect

Returns the bounding rectangle for the glyphs in the specified text container.

