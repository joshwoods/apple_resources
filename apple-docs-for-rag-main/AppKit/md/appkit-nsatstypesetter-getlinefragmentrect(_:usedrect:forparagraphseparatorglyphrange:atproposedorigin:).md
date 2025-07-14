

- AppKit
- NSATSTypesetter
-  getLineFragmentRect(\_:usedRect:forParagraphSeparatorGlyphRange:atProposedOrigin:) 

Instance Method

# getLineFragmentRect(\_:usedRect:forParagraphSeparatorGlyphRange:atProposedOrigin:)

Calculates the line fragment rectangle and the portion of the rectangle that contains marks.

macOS

``` source
func getLineFragmentRect(
    _ lineFragmentRect: UnsafeMutablePointer,
    usedRect lineFragmentUsedRect: UnsafeMutablePointer,
    forParagraphSeparatorGlyphRange paragraphSeparatorGlyphRange: NSRange,
    atProposedOrigin lineOrigin: NSPoint
)
```

## Discussion

The method returns the calculated line fragment rectangle in `lineFragmentRect`, and it returns the used rectangle (the portion of the line fragment rectangle that actually contains marks) in `lineFragmentUsedRect`. The `paragraphSeparatorGlyphRange` is the range of glyphs under consideration, and `lineOrigin` is the origin point of the line fragment rectangle. A `paragraphSeparatorGlyphRange` with length 0 indicates an extra line fragment (which occurs if the last character in the paragraph is a line separator.)

## See Also

### Laying Out Glyphs

func boundingBox(forControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the bounding rectangle for a control glyph, at the specified glyph position and character index in the text container.

func hyphenCharacter(forGlyphAt: Int) -> UTF32Char

Returns the hyphen character to be inserted after the specified glyph when hyphenation is enabled in the layout manager.

func hyphenationFactor(forGlyphAt: Int) -> Float

Returns the hyphenation factor in effect at the specified glyph index.

func shouldBreakLine(byHyphenatingBeforeCharacterAt: Int) -> Bool

Breaks a line by hyphenating before the character at the specified index.

func shouldBreakLine(byWordBeforeCharacterAt: Int) -> Bool

Breaks a line by word-wrapping before the character at the specified index.

func willSetLineFragmentRect(UnsafeMutablePointer&lt;NSRect>, forGlyphRange: NSRange, usedRect: UnsafeMutablePointer&lt;NSRect>, baselineOffset: UnsafeMutablePointer&lt;CGFloat>)

Notifies subclasses that the typesetter is about to set a new line fragment.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets a Boolean value that determines whether the layout manager invalidates the specified portion of the glyph cache.

