

- AppKit
- NSATSTypesetter
-  shouldBreakLine(byHyphenatingBeforeCharacterAt:) 

Instance Method

# shouldBreakLine(byHyphenatingBeforeCharacterAt:)

Breaks a line by hyphenating before the character at the specified index.

macOS

``` source
func shouldBreakLine(byHyphenatingBeforeCharacterAt charIndex: Int) -> Bool
```

## Discussion

The typesetter calls this method, if implemented by a subclass, before breaking a line by hyphenating before the character at the given character index, enabling the subclass to control line breaking. A subclass can override this method to customize the text layout process. If the method returns false, the typesetter continues looking for a break point.

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

func shouldBreakLine(byWordBeforeCharacterAt: Int) -> Bool

Breaks a line by word-wrapping before the character at the specified index.

func willSetLineFragmentRect(UnsafeMutablePointer&lt;NSRect>, forGlyphRange: NSRange, usedRect: UnsafeMutablePointer&lt;NSRect>, baselineOffset: UnsafeMutablePointer&lt;CGFloat>)

Notifies subclasses that the typesetter is about to set a new line fragment.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets a Boolean value that determines whether the layout manager invalidates the specified portion of the glyph cache.

