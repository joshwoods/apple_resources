

- AppKit
-  NSATSTypesetter 

Class

# NSATSTypesetter

A concrete typesetter object that places glyphs during the text layout process.

macOS

``` source
class NSATSTypesetter
```

## Overview

An NSATSTypesetter object creates line fragment rectangles, positions glyphs within the line fragments, determines line breaks by word wrapping and hyphenation, and handles tab positioning. This object encapsulates the advanced typesetting capabilities of Core Text. NSATSTypesetter provides line and character spacing accuracy and supports many languages, including bidirectional languages.

Note

Use this class with NSLayoutManager in macOS11 and earlier. In macOS12 and later, consider using NSTextLayoutManager which provides improved support for international scripts.

## Topics

### Getting the shared typesetter object

class var shared: NSATSTypesetter

Returns a shared instance of the typesetter.

### Accessing the layout manager

var layoutManager: NSLayoutManager?

The layout manager for the text being typeset.

var usesFontLeading: Bool

A Boolean value controlling whether the typesetter uses the leading (or line gap) value specified in the font metric information.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

The current typesetter behavior value.

var hyphenationFactor: Float

The threshold controlling when hyphenation is attempted.

var bidiProcessingEnabled: Bool

A Boolean value controlling whether the typesetter performs bidirectional text processing.

### Getting the text container

var currentTextContainer: NSTextContainer?

The text container for the text being typeset.

var lineFragmentPadding: CGFloat

The amount (in points) by which text is inset within line fragment rectangles.

### Performing font substitution

func substituteFont(for: NSFont) -> NSFont

Returns a screen font suitable for use in place of the specified original font,.

### Getting the location of text tabs

func textTab(forGlyphLocation: CGFloat, writingDirection: NSWritingDirection, maxLocation: CGFloat) -> NSTextTab?

Returns the text tab closest to the specified glyph location and not beyond a maximum position.

### Accessing paragraph information

var attributedString: NSAttributedString?

The backing store that contains the text on which this typesetter operates.

func setParagraphGlyphRange(NSRange, separatorGlyphRange: NSRange)

Sets the glyph range being processed and the paragraph separator glyph range (the range of the paragraph separator character or characters).

var paragraphGlyphRange: NSRange

The current glyph range being processed.

var paragraphSeparatorGlyphRange: NSRange

The current paragraph separator range that contains the current glyph range and extends from one paragraph separator character to the next.

### Laying out a paragraph

func layoutParagraph(at: UnsafeMutablePointer&lt;NSPoint>) -> Int

Lays out glyphs in the current glyph range until the next paragraph separator is reached.

### Getting Spacing Information

func lineSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the line spacing in effect following the specified glyph.

func paragraphSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the number of points of space added following a paragraph, in effect after the specified glyph.

func paragraphSpacing(beforeGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the number of points of space added before a paragraph, which is in effect before the specified glyph.

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

func willSetLineFragmentRect(UnsafeMutablePointer&lt;NSRect>, forGlyphRange: NSRange, usedRect: UnsafeMutablePointer&lt;NSRect>, baselineOffset: UnsafeMutablePointer&lt;CGFloat>)

Notifies subclasses that the typesetter is about to set a new line fragment.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets a Boolean value that determines whether the layout manager invalidates the specified portion of the glyph cache.

### Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>!, characterIndexes: UnsafeMutablePointer&lt;Int>!, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>!, elasticBits: UnsafeMutablePointer&lt;ObjCBool>!) -> Int

Extracts the information needed to lay out the glyphs in the given glyph buffer from the given glyph range.

Deprecated

## Relationships

### Inherits From

- NSTypesetter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### TextKit 1

class NSTextStorage

The fundamental storage mechanism of TextKit that contains the text managed by the system.

class NSLayoutManager

An object that coordinates the layout and display of text characters.

class NSTypesetter

An abstract class that performs various type layout tasks.

