

- AppKit
- NSATSTypesetter
-  hyphenationFactor(forGlyphAt:) 

Instance Method

# hyphenationFactor(forGlyphAt:)

Returns the hyphenation factor in effect at the specified glyph index.

macOS

``` source
func hyphenationFactor(forGlyphAt glyphIndex: Int) -> Float
```

## Discussion

The hyphenation factor is a value ranging from 0.0 to 1.0 that controls when hyphenation is attempted. By default, the value is 0.0, meaning hyphenation is off. A factor of 1.0 causes hyphenation to be attempted always.

The typesetter calls this method with a proposed hyphenation point for a line break to find the hyphenation factor in effect at that time. A subclass can override this method to customize the text layout process.

## See Also

### Laying Out Glyphs

func boundingBox(forControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the bounding rectangle for a control glyph, at the specified glyph position and character index in the text container.

func getLineFragmentRect(UnsafeMutablePointer&lt;NSRect>, usedRect: UnsafeMutablePointer&lt;NSRect>, forParagraphSeparatorGlyphRange: NSRange, atProposedOrigin: NSPoint)

Calculates the line fragment rectangle and the portion of the rectangle that contains marks.

func hyphenCharacter(forGlyphAt: Int) -> UTF32Char

Returns the hyphen character to be inserted after the specified glyph when hyphenation is enabled in the layout manager.

func shouldBreakLine(byHyphenatingBeforeCharacterAt: Int) -> Bool

Breaks a line by hyphenating before the character at the specified index.

func shouldBreakLine(byWordBeforeCharacterAt: Int) -> Bool

Breaks a line by word-wrapping before the character at the specified index.

func willSetLineFragmentRect(UnsafeMutablePointer&lt;NSRect>, forGlyphRange: NSRange, usedRect: UnsafeMutablePointer&lt;NSRect>, baselineOffset: UnsafeMutablePointer&lt;CGFloat>)

Notifies subclasses that the typesetter is about to set a new line fragment.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets a Boolean value that determines whether the layout manager invalidates the specified portion of the glyph cache.

