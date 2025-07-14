

- UIKit
-  NSLayoutManagerDelegate 

Protocol

# NSLayoutManagerDelegate

A set of optional methods that delegates of layout manager objects implement.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
protocol NSLayoutManagerDelegate : NSObjectProtocol
```

## Topics

### Invalidating glyphs and layout

func layoutManagerDidInvalidateLayout(NSLayoutManager)

Informs the delegate when the specified layout manager invalidates layout information (not glyph information).

func layoutManager(NSLayoutManager, shouldGenerateGlyphs: UnsafePointer&lt;CGGlyph>, properties: UnsafePointer&lt;NSLayoutManager.GlyphProperty>, characterIndexes: UnsafePointer&lt;Int>, font: UIFont, forGlyphRange: NSRange) -> Int

Enables customization of the initial glyph generation process.

func layoutManager(NSLayoutManager, shouldUse: NSLayoutManager.ControlCharacterAction, forControlCharacterAt: Int) -> NSLayoutManager.ControlCharacterAction

Returns the control character action for the control character at the specified character index.

struct ControlCharacterAction

Constants that describe actions for control characters.

### Responding to text container layout

func layoutManager(NSLayoutManager, didCompleteLayoutFor: NSTextContainer?, atEnd: Bool)

Informs the delegate when the layout manager finishes laying out text in the specified text container.

func layoutManager(NSLayoutManager, textContainer: NSTextContainer, didChangeGeometryFrom: CGSize)

Informs the delegate when the layout manager invalidates layout due to a change in the geometry of the specified text container.

### Handling line fragments

func layoutManager(NSLayoutManager, shouldBreakLineByHyphenatingBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified character.

func layoutManager(NSLayoutManager, shouldBreakLineByWordBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified word.

func layoutManager(NSLayoutManager, lineSpacingAfterGlyphAt: Int, withProposedLineFragmentRect: CGRect) -> CGFloat

Returns the amount of space to add to the end of a line.

func layoutManager(NSLayoutManager, paragraphSpacingAfterGlyphAt: Int, withProposedLineFragmentRect: CGRect) -> CGFloat

Returns the amount of space to add at the end of a paragraph.

func layoutManager(NSLayoutManager, paragraphSpacingBeforeGlyphAt: Int, withProposedLineFragmentRect: CGRect) -> CGFloat

Returns the amount of space to add at the beginning of a paragraph.

func layoutManager(NSLayoutManager, boundingBoxForControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: CGRect, glyphPosition: CGPoint, characterIndex: Int) -> CGRect

Returns the bounding rectangle for the specified control glyph with the specified parameters.

func layoutManager(NSLayoutManager, shouldSetLineFragmentRect: UnsafeMutablePointer&lt;CGRect>, lineFragmentUsedRect: UnsafeMutablePointer&lt;CGRect>, baselineOffset: UnsafeMutablePointer&lt;CGFloat>, in: NSTextContainer, forGlyphRange: NSRange) -> Bool

Customizes the line fragment geometry before committing it to the layout cache.

### Managing temporary attribute support

optional func layoutManager(_ layoutManager: NSLayoutManager, shouldUseTemporaryAttributes attrs: [NSAttributedString.Key : Any] = [:], forDrawingToScreen toScreen: Bool, atCharacterIndex charIndex: Int, effectiveRange effectiveCharRange: NSRangePointer?) -> [NSAttributedString.Key : Any]?

Asks the delegate whether to use temporary attributes when drawing the text.

### Deprecated

Control Characters

Constants that describe actions for control characters.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing the layout process

var delegate: (any NSLayoutManagerDelegate)?

The layout manager’s delegate.

