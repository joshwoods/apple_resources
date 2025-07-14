

- AppKit
- NSATSTypesetter
-  willSetLineFragmentRect(\_:forGlyphRange:usedRect:baselineOffset:) 

Instance Method

# willSetLineFragmentRect(\_:forGlyphRange:usedRect:baselineOffset:)

Notifies subclasses that the typesetter is about to set a new line fragment.

macOS

``` source
func willSetLineFragmentRect(
    _ lineRect: UnsafeMutablePointer,
    forGlyphRange glyphRange: NSRange,
    usedRect: UnsafeMutablePointer,
    baselineOffset: UnsafeMutablePointer
)
```

## Discussion

The typesetter calls this method before calling setLineFragmentRect(_:forGlyphRange:usedRect:), which stores the actual line fragment rectangle location in the layout manager.

The `lineRect` argument is the rectangle in which the glyphs in `glyphRange` are laid out. The `usedRect` argument indicates the portion of `lineRect`, in the NSTextContainer object’s coordinate system, that actually contains glyphs or other marks that are drawn (including the text container’s line fragment padding). The `usedRect` must be equal to or contained within `lineRect`. The `baselineOffset` argument is the vertical distance in pixels from the line fragment origin to the baseline on which the glyphs align.

A subclass can override this method to customize the text layout process. For example, it could change the shape of the line fragment rectangle. The subclass is responsible for ensuring that the modified rectangle remains valid (for example, that it lies within the text container).

## See Also

### Laying Out Glyphs

func boundingBox(forControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the bounding rectangle for a control glyph, at the specified glyph position and character index in the text container.

func getLineFragmentRect(UnsafeMutablePointer&lt;NSRect>, usedRect: UnsafeMutablePointer&lt;NSRect>, forParagraphSeparatorGlyphRange: NSRange, atProposedOrigin: NSPoint)

Calculates the line fragment rectangle and the portion of the rectangle that contains marks.

func hyphenCharacter(forGlyphAt: Int) -> UTF32Char

Returns the hyphen character to be inserted after the specified glyph when hyphenation is enabled in the layout manager.

func hyphenationFactor(forGlyphAt: Int) -> Float

Returns the hyphenation factor in effect at the specified glyph index.

func shouldBreakLine(byHyphenatingBeforeCharacterAt: Int) -> Bool

Breaks a line by hyphenating before the character at the specified index.

func shouldBreakLine(byWordBeforeCharacterAt: Int) -> Bool

Breaks a line by word-wrapping before the character at the specified index.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets a Boolean value that determines whether the layout manager invalidates the specified portion of the glyph cache.

