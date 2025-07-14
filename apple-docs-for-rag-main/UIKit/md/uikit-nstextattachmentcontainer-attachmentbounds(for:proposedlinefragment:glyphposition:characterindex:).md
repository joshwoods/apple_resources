

- UIKit
- NSTextAttachmentContainer
-  attachmentBounds(for:proposedLineFragment:glyphPosition:characterIndex:) 

Instance Method

# attachmentBounds(for:proposedLineFragment:glyphPosition:characterIndex:)

Returns the layout bounds of the text attachment to the layout manager.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func attachmentBounds(
    for textContainer: NSTextContainer?,
    proposedLineFragment lineFrag: CGRect,
    glyphPosition position: CGPoint,
    characterIndex charIndex: Int
) -> CGRect
```

**Required**

## Parameters 

`textContainer`  

The text container for the text being laid out.

`lineFrag`  

The line fragment containing the text attachment.

`position`  

The glyph location inside `lineFrag` which is the origin of the returned bounds rectangle.

`charIndex`  

The character location inside the text storage for the attachment character.

## Return Value

The bounds rectangle of the text attachment if not CGRectZero; otherwise, the rectangle of the size property of the attachment’s image property.

## Discussion

Conforming objects can implement more sophisticated logic for negotiating the attachment bounds based on the available container space and proposed line fragment rectangle.

