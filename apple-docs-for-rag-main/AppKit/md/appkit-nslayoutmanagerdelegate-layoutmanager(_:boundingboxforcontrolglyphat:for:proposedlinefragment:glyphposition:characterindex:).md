

- AppKit
- NSLayoutManagerDelegate
-  layoutManager(\_:boundingBoxForControlGlyphAt:for:proposedLineFragment:glyphPosition:characterIndex:) 

Instance Method

# layoutManager(\_:boundingBoxForControlGlyphAt:for:proposedLineFragment:glyphPosition:characterIndex:)

Returns the bounding rectangle for the specified control glyph with the specified parameters.

macOS 10.11+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    boundingBoxForControlGlyphAt glyphIndex: Int,
    for textContainer: NSTextContainer,
    proposedLineFragment proposedRect: NSRect,
    glyphPosition: NSPoint,
    characterIndex charIndex: Int
) -> NSRect
```

## Parameters 

`layoutManager`  

The layout manager doing the layout.

`glyphIndex`  

The index of the control glyph in question.

`textContainer`  

The text container to use to calculate the position.

`proposedRect`  

The proposed line fragment rectangle.

`glyphPosition`  

The position of the glyph in `textContainer`.

`charIndex`  

The character index in `textContainer`.

## Return Value

The bounding rectangle for the specified control glyph with the specified parameters.

## Discussion

Sent for resolving the glyph metrics for NSControlCharacterWhitespaceAction control character.

## See Also

### Handling line fragments

func layoutManager(NSLayoutManager, shouldBreakLineByHyphenatingBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified character.

func layoutManager(NSLayoutManager, shouldBreakLineByWordBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified word.

func layoutManager(NSLayoutManager, lineSpacingAfterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the amount of space to add to the end of a line.

func layoutManager(NSLayoutManager, paragraphSpacingAfterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the amount of space to add at the end of a paragraph.

func layoutManager(NSLayoutManager, paragraphSpacingBeforeGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the amount of space to add at the beginning of a paragraph.

func layoutManager(NSLayoutManager, shouldSetLineFragmentRect: UnsafeMutablePointer&lt;NSRect>, lineFragmentUsedRect: UnsafeMutablePointer&lt;NSRect>, baselineOffset: UnsafeMutablePointer&lt;CGFloat>, in: NSTextContainer, forGlyphRange: NSRange) -> Bool

Customizes the line fragment geometry before committing it to the layout cache.

