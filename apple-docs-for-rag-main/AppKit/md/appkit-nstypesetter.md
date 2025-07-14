

- AppKit
-  NSTypesetter 

Class

# NSTypesetter

An abstract class that performs various type layout tasks.

macOS

``` source
class NSTypesetter
```

## Overview

NSLayoutManager uses concrete subclasses of NSTypesetter to perform line layout, which includes word wrapping, hyphenation, and line breaking in either vertical or horizontal rectangles. By default, the text system uses the concrete subclass NSATSTypesetter.

Note

Use this class with NSLayoutManager in macOS11 and earlier. In macOS12 and later, consider using NSLayoutManager which provides improved support for international scripts.

### Subclassing Notes

`NSTypesetter` provides concrete subclasses with default implementation interfacing with the Cocoa text system. By subclassing `NSTypesetter`, an application can override the layoutParagraph(at:) method to integrate a custom typesetting engine into the Cocoa text system. On the other hand, an application can subclass NSATSTypesetter and override the glyph storage interface to integrate the concrete subclass into its own custom layout system.

`NSTypesetter` methods belong to three categories: glyph storage interface methods, layout phase interface methods, and core typesetter methods. The glyph storage interface methods map to NSLayoutManager methods. The typesetter itself calls these methods, and their default implementations call the Cocoa layout manager. An `NSTypesetter` subclass can override these methods to call its own glyph storage facility, in which case it should override all of them. (This doesn’t preclude the overridden method calling its superclass implementation if appropriate).

The layout phase interface provides control points similar to delegate methods; if implemented, the system invokes these methods to notify an `NSTypesetter` subclass of events in the layout process so it can intervene as needed.

The remainder of the `NSTypesetter` methods are primitive, core typesetter methods. The core typesetter methods correlate with typesetting state attributes; the layout manager calls these methods to store its values before starting the layout process. If you subclass `NSTypesetter` and override the glyph storage interface methods, you can call the core methods to control the typesetter directly.

#### Glyph Storage Interface

Override these methods to use `NSTypesetter`’s built-in concrete subclass, NSATSTypesetter, with a custom glyph storage and layout system other than the Cocoa layout manager and text container mechanism.

- characterRange(forGlyphRange:actualGlyphRange:)

- glyphRange(forCharacterRange:actualCharacterRange:)

- getGlyphs(in:glyphs:characterIndexes:glyphInscriptions:elasticBits:bidiLevels:)

- getLineFragmentRect(_:usedRect:remaining:forStartingGlyphAt:proposedRect:lineSpacing:paragraphSpacingBefore:paragraphSpacingAfter:)

- setLineFragmentRect(_:forGlyphRange:usedRect:baselineOffset:)

- substituteGlyphs(in:withGlyphs:)

- insertGlyph(_:atGlyphIndex:characterIndex:)

- deleteGlyphs(in:)

- setNotShownAttribute(_:forGlyphRange:)

- setDrawsOutsideLineFragment(_:forGlyphRange:)

- setLocation(_:withAdvancements:forStartOfGlyphRange:)

- setAttachmentSize(_:forGlyphRange:)

- setBidiLevels(_:forGlyphRange:)

#### Layout Phase Interface

Override these methods to customize the text layout process, including modifying line fragments, controlling line breaking and hyphenation, and controlling the behavior of tabs and other control glyphs.

- willSetLineFragmentRect(_:forGlyphRange:usedRect:baselineOffset:)

- shouldBreakLine(byWordBeforeCharacterAt:)

- shouldBreakLine(byHyphenatingBeforeCharacterAt:)

- hyphenationFactor(forGlyphAt:)

- hyphenCharacter(forGlyphAt:)

- boundingBox(forControlGlyphAt:for:proposedLineFragment:glyphPosition:characterIndex:)

## Topics

### Getting a typesetter

class var sharedSystemTypesetter: NSTypesetter

Returns a shared instance of a reentrant typesetter.

class func sharedSystemTypesetter(for: NSLayoutManager.TypesetterBehavior) -> Any

Returns a shared instance of a reentrant typesetter that implements typesetting with the specified behavior.

### Getting information about a typesetter

class var defaultTypesetterBehavior: NSLayoutManager.TypesetterBehavior

Returns the default typesetter behavior.

### Getting information about glyphs

class func printingAdjustment(in: NSLayoutManager, forNominallySpacedGlyphRange: NSRange, packedGlyphs: UnsafePointer&lt;UInt8>, count: Int) -> NSSize

Returns the interglyph spacing in the specified range when sent to a printer.

func baselineOffset(in: NSLayoutManager, glyphIndex: Int) -> CGFloat

Returns the distance from the bottom of the line fragment rectangle in which the glyph resides to the glyph baseline.

### Accessing the layout manager

var layoutManager: NSLayoutManager?

Returns the layout manager for the text being typeset.

var usesFontLeading: Bool

Returns whether the typesetter uses the leading (or line gap) value specified in the font metric information of the current font.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

Returns the current typesetter behavior.

var hyphenationFactor: Float

Returns the current hyphenation factor.

### Managing text containers

var currentTextContainer: NSTextContainer?

Returns the text container for the text being typeset.

var textContainers: NSArray?

Returns an array containing the text containers belonging to the current layout manager.

var lineFragmentPadding: CGFloat

Returns the current line fragment padding, in points.

### Performing font substitution

func substituteFont(for: NSFont) -> NSFont

Returns a screen font suitable for use in place of a given font.

### Getting the location of text tabs

func textTab(forGlyphLocation: CGFloat, writingDirection: NSWritingDirection, maxLocation: CGFloat) -> NSTextTab?

Returns the text tab next closest to a given glyph location within the given parameters.

### Bidirectional text processing

var bidiProcessingEnabled: Bool

Returns whether bidirectional text processing is enabled.

### Accessing paragraph typesetting information

var currentParagraphStyle: NSParagraphStyle?

Returns the paragraph style object for the text being typeset.

var attributedString: NSAttributedString?

Returns the text backing store, usually an instance of `NSTextStorage`.

func setParagraphGlyphRange(NSRange, separatorGlyphRange: NSRange)

Sets the current glyph range being processed.

var paragraphGlyphRange: NSRange

Returns the glyph range currently being processed.

var paragraphSeparatorGlyphRange: NSRange

Returns the current paragraph separator range.

var paragraphCharacterRange: NSRange

Returns the character range currently being processed.

var paragraphSeparatorCharacterRange: NSRange

Returns the current paragraph separator character range.

var attributesForExtraLineFragment: [NSAttributedString.Key : Any]

Returns the attributes used to lay out the extra line fragment.

### Getting spacing information

func lineSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the line spacing in effect following the specified glyph.

func paragraphSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the paragraph spacing that is in effect after the specified glyph.

func paragraphSpacing(beforeGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the number of points of space—added before a paragraph—that is in effect before the specified glyph.

### Laying out a paragraph

func layoutParagraph(at: NSPointPointer) -> Int

Lays out glyphs in the current glyph range until the next paragraph separator is reached.

func beginParagraph()

Sets up layout parameters at the beginning of a paragraph.

func endParagraph()

Sets up layout parameters at the end of a paragraph.

func beginLine(withGlyphAt: Int)

Sets up layout parameters at the beginning of a line during typesetting.

func endLine(withGlyphRange: NSRange)

Sets up layout parameters at the end of a line during typesetting.

### Laying out characters

func layoutCharacters(in: NSRange, for: NSLayoutManager, maximumNumberOfLineFragments: Int) -> NSRange

Lays out characters in the given character range for the specified layout manager.

### Laying out glyphs

func layoutGlyphs(in: NSLayoutManager, startingAtGlyphIndex: Int, maxNumberOfLineFragments: Int, nextGlyphIndex: UnsafeMutablePointer&lt;Int>)

Lays out glyphs in the specified layout manager starting at a specified glyph.

Deprecated

func boundingBox(forControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the bounding rectangle for the specified control glyph with the specified parameters.

func getLineFragmentRect(NSRectPointer, usedRect: NSRectPointer, forParagraphSeparatorGlyphRange: NSRange, atProposedOrigin: NSPoint)

Calculates the line fragment rectangle and line fragment used rectangle for blank lines.

func getLineFragmentRect(NSRectPointer!, usedRect: NSRectPointer!, remaining: NSRectPointer!, forStartingGlyphAt: Int, proposedRect: NSRect, lineSpacing: CGFloat, paragraphSpacingBefore: CGFloat, paragraphSpacingAfter: CGFloat)

Calculates line fragment rectangle, line fragment used rectangle, and remaining rectangle for a line fragment.

func hyphenCharacter(forGlyphAt: Int) -> UTF32Char

Returns the hyphen character to be inserted after the specified glyph.

func hyphenationFactor(forGlyphAt: Int) -> Float

Returns the hyphenation factor in effect at a specified location.

func shouldBreakLine(byHyphenatingBeforeCharacterAt: Int) -> Bool

Returns whether the line being laid out should be broken by hyphenating at the specified character.

func shouldBreakLine(byWordBeforeCharacterAt: Int) -> Bool

Returns whether the line being laid out should be broken by a word break at the specified character.

func willSetLineFragmentRect(NSRectPointer, forGlyphRange: NSRange, usedRect: NSRectPointer, baselineOffset: UnsafeMutablePointer&lt;CGFloat>)

Called by the typesetter just prior to storing the actual line fragment rectangle location in the layout manager.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets whether to force the layout manager to invalidate the specified portion of the glyph cache when invalidating layout.

### Interfacing with Glyph Storage

func characterRange(forGlyphRange: NSRange, actualGlyphRange: NSRangePointer?) -> NSRange

Returns the range for the characters in the receiver’s text store that are mapped to the specified glyphs.

func glyphRange(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?) -> NSRange

Returns the range for the glyphs mapped to the characters of the text store in the specified range.

func setAttachmentSize(NSSize, forGlyphRange: NSRange)

Sets the size the specified glyphs (assumed to be attachments) will be asked to draw themselves at.

func setBidiLevels(UnsafePointer&lt;UInt8>!, forGlyphRange: NSRange)

Sets the direction of the specified glyphs for bidirectional text.

func setDrawsOutsideLineFragment(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs exceed the bounds of the line fragment in which they are laid out.

func setLineFragmentRect(NSRect, forGlyphRange: NSRange, usedRect: NSRect, baselineOffset: CGFloat)

Sets the line fragment rectangle where the specified glyphs are laid out.

func setLocation(NSPoint, withAdvancements: UnsafePointer&lt;CGFloat>!, forStartOfGlyphRange: NSRange)

Sets the location where the specified glyphs are laid out.

func setNotShownAttribute(Bool, forGlyphRange: NSRange)

Sets whether the specified glyphs are not shown.

### Deprecated

func actionForControlCharacter(at: Int) -> NSTypesetterControlCharacterAction

Returns the action associated with a control character.

func deleteGlyphs(in: NSRange)

Deletes the specified glyphs from the glyph cache maintained by the layout manager.

Deprecated

func substituteGlyphs(in: NSRange, withGlyphs: UnsafeMutablePointer&lt;NSGlyph>!)

Replaces the specified glyphs with specified replacement glyphs.

Deprecated

func getGlyphs(in: NSRange, glyphs: UnsafeMutablePointer&lt;NSGlyph>!, characterIndexes: UnsafeMutablePointer&lt;Int>!, glyphInscriptions: UnsafeMutablePointer&lt;NSGlyphInscription>!, elasticBits: UnsafeMutablePointer&lt;ObjCBool>!, bidiLevels: UnsafeMutablePointer&lt;UInt8>!) -> Int

Extracts the information needed to lay out the provided glyphs from the provided range.

Deprecated

func insertGlyph(NSGlyph, atGlyphIndex: Int, characterIndex: Int)

Enables the typesetter to insert a new glyph into the stream.

Deprecated

struct NSTypesetterControlCharacterAction

The following constants are possible values returned by the actionForControlCharacter(at:) method to determine the action associated with a control character.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSATSTypesetter

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

class NSATSTypesetter

A concrete typesetter object that places glyphs during the text layout process.

