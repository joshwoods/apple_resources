

- UIKit
- NSLayoutManagerDelegate
-  layoutManager(\_:paragraphSpacingAfterGlyphAt:withProposedLineFragmentRect:) 

Instance Method

# layoutManager(\_:paragraphSpacingAfterGlyphAt:withProposedLineFragmentRect:)

Returns the amount of space to add at the end of a paragraph.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    paragraphSpacingAfterGlyphAt glyphIndex: Int,
    withProposedLineFragmentRect rect: CGRect
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

The paragraph spacing after the current line.

## Discussion

This message is sent while each line is laid out to enable the layout manager delegate to customize the shape of line.

## See Also

### Handling line fragments

func layoutManager(NSLayoutManager, shouldBreakLineByHyphenatingBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified character.

func layoutManager(NSLayoutManager, shouldBreakLineByWordBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified word.

func layoutManager(NSLayoutManager, lineSpacingAfterGlyphAt: Int, withProposedLineFragmentRect: CGRect) -> CGFloat

Returns the amount of space to add to the end of a line.

func layoutManager(NSLayoutManager, paragraphSpacingBeforeGlyphAt: Int, withProposedLineFragmentRect: CGRect) -> CGFloat

Returns the amount of space to add at the beginning of a paragraph.

func layoutManager(NSLayoutManager, boundingBoxForControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: CGRect, glyphPosition: CGPoint, characterIndex: Int) -> CGRect

Returns the bounding rectangle for the specified control glyph with the specified parameters.

func layoutManager(NSLayoutManager, shouldSetLineFragmentRect: UnsafeMutablePointer&lt;CGRect>, lineFragmentUsedRect: UnsafeMutablePointer&lt;CGRect>, baselineOffset: UnsafeMutablePointer&lt;CGFloat>, in: NSTextContainer, forGlyphRange: NSRange) -> Bool

Customizes the line fragment geometry before committing it to the layout cache.

