

- AppKit
- NSLayoutManagerDelegate
-  layoutManager(\_:lineSpacingAfterGlyphAt:withProposedLineFragmentRect:) 

Instance Method

# layoutManager(\_:lineSpacingAfterGlyphAt:withProposedLineFragmentRect:)

Returns the amount of space to add to the end of a line.

macOS 10.11+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    lineSpacingAfterGlyphAt glyphIndex: Int,
    withProposedLineFragmentRect rect: NSRect
) -> CGFloat
```

## Parameters 

`layoutManager`  

The layout manager doing the layout.

`glyphIndex`  

The index of the glyph at the end of the line.

`rect`  

The proposed line fragment rectangle for the current line.

## Return Value

The line spacing after the current line.

## Discussion

This message is sent while each line is laid out to enable the layout manager delegate to customize the shape of line.

## See Also

### Handling line fragments

func layoutManager(NSLayoutManager, shouldBreakLineByHyphenatingBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified character.

func layoutManager(NSLayoutManager, shouldBreakLineByWordBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified word.

func layoutManager(NSLayoutManager, paragraphSpacingAfterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the amount of space to add at the end of a paragraph.

func layoutManager(NSLayoutManager, paragraphSpacingBeforeGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the amount of space to add at the beginning of a paragraph.

func layoutManager(NSLayoutManager, boundingBoxForControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the bounding rectangle for the specified control glyph with the specified parameters.

func layoutManager(NSLayoutManager, shouldSetLineFragmentRect: UnsafeMutablePointer&lt;NSRect>, lineFragmentUsedRect: UnsafeMutablePointer&lt;NSRect>, baselineOffset: UnsafeMutablePointer&lt;CGFloat>, in: NSTextContainer, forGlyphRange: NSRange) -> Bool

Customizes the line fragment geometry before committing it to the layout cache.

