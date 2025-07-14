

- UIKit
- NSLayoutManagerDelegate
-  layoutManager(\_:shouldSetLineFragmentRect:lineFragmentUsedRect:baselineOffset:in:forGlyphRange:) 

Instance Method

# layoutManager(\_:shouldSetLineFragmentRect:lineFragmentUsedRect:baselineOffset:in:forGlyphRange:)

Customizes the line fragment geometry before committing it to the layout cache.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    shouldSetLineFragmentRect lineFragmentRect: UnsafeMutablePointer,
    lineFragmentUsedRect: UnsafeMutablePointer,
    baselineOffset: UnsafeMutablePointer,
    in textContainer: NSTextContainer,
    forGlyphRange glyphRange: NSRange
) -> Bool
```

## Parameters 

`layoutManager`  

The layout manager doing the work.

`lineFragmentRect`  

The proposed rectangle that contains the glyphs. You may modify this rectangle as needed.

`lineFragmentUsedRect`  

The portion of `lineFragmentRect` that actually contains glyphs or other rendered marks, including the text container’s line fragment padding. This rectangle must be equal to `lineFragmentRect` or wholly contained by it. You may modify this rectangle as needed.

`baselineOffset`  

The vertical distance (in pixels) from the line fragment origin to the baseline on which the glyphs align.

`textContainer`  

The text container for the line fragments.

`glyphRange`  

The range of glyphs being laid out.

## Return Value

true if you modified the layout information and want your modifications to be used or false if the original layout information should be used.

## Discussion

Use this method to modify the line fragment rectangles associated with the text container. It is your responsibility to ensure that the modified rectangles remain valid and still lie within the text container.

## See Also

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

