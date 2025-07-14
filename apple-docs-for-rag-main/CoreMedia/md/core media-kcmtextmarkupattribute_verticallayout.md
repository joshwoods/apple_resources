

- Core Media
-  kCMTextMarkupAttribute_VerticalLayout 

Global Variable

# kCMTextMarkupAttribute_VerticalLayout

The vertical layout of a text block.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAttribute_VerticalLayout: CFString
```

## Discussion

Specifying this attribute indicates that the writing direction is vertical instead of horizontal. You can set the associated value to kCMTextVerticalLayout_LeftToRight or kCMTextVerticalLayout_RightToLeft to indicate the progression direction for new vertical lines of text.

## Topics

### Layouts

let kCMTextVerticalLayout_LeftToRight: CFString

Add new vertical lines from left to right.

let kCMTextVerticalLayout_RightToLeft: CFString

Add new vertical lines from right to left.

## See Also

### Layout

let kCMTextMarkupAttribute_Alignment: CFString

The text alignment in the writing direction of the first line of text.

let kCMTextMarkupAttribute_TextPositionPercentageRelativeToWritingDirection: CFString

The placement of the block of text as a percentage in the writing direction.

let kCMTextMarkupAttribute_OrthogonalLinePositionPercentageRelativeToWritingDirection: CFString

The placement of the first line in a block of text as a percentage in the direction orthogonal to the writing direction.

let kCMTextMarkupAttribute_WritingDirectionSizePercentage: CFString

The width or height as a percentage of the bounding box that contains the text.

