

- AppKit
- NSLayoutManager
-  textContainerChangedGeometry(\_:) 

Instance Method

# textContainerChangedGeometry(\_:)

Invalidates the layout information, and possibly glyphs, for the specified text container and all subsequent text container objects.

macOS 10.7+

``` source
func textContainerChangedGeometry(_ container: NSTextContainer)
```

## Parameters 

`container`  

The text container whose layout is invalidated.

## Discussion

This method is invoked automatically by other components of the text system; you should rarely need to invoke it directly. Subclasses of `NSTextContainer`, however, must invoke this method any time their size of shape changes (a text container that dynamically adjusts its shape to wrap text around placed graphics, for example, must do so when a graphic is added, moved, or removed).

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

func textContainerChangedTextView(NSTextContainer)

Updates the information necessary to manage text view objects for the specified text container.

func textContainer(forGlyphAt: Int, effectiveRange: NSRangePointer?) -> NSTextContainer?

Returns the text container that manages the layout for the specified glyph, causing layout to happen as necessary.

func textContainer(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> NSTextContainer?

Returns the text container that manages the layout for the specified glyph.

func usedRect(for: NSTextContainer) -> NSRect

Returns the bounding rectangle for the glyphs in the specified text container.

