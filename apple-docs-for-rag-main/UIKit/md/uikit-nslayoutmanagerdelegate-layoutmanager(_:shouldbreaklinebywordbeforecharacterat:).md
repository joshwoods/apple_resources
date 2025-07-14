

- UIKit
- NSLayoutManagerDelegate
-  layoutManager(\_:shouldBreakLineByWordBeforeCharacterAt:) 

Instance Method

# layoutManager(\_:shouldBreakLineByWordBeforeCharacterAt:)

Asks the delegate whether to break the line at the specified word.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    shouldBreakLineByWordBeforeCharacterAt charIndex: Int
) -> Bool
```

## Parameters 

`layoutManager`  

The layout manager doing the layout.

`charIndex`  

Index of the character delimiting the break point search.

## Return Value

true if the current line break point is acceptable; false if the layout manager should find the next break point opportunity before `charIndex`.

## See Also

### Handling line fragments

func layoutManager(NSLayoutManager, shouldBreakLineByHyphenatingBeforeCharacterAt: Int) -> Bool

Asks the delegate whether to break the line at the specified character.

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

