

- Core Media
-  kCMTextMarkupAttribute_OrthogonalLinePositionPercentageRelativeToWritingDirection 

Global Variable

# kCMTextMarkupAttribute_OrthogonalLinePositionPercentageRelativeToWritingDirection

The placement of the first line in a block of text as a percentage in the direction orthogonal to the writing direction.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAttribute_OrthogonalLinePositionPercentageRelativeToWritingDirection: CFString
```

## Discussion

This attribute’s value must be a non-negative `CFNumber` that expresses the position of the center of the cue relative to the writing direction. The line position is orthogonal (or perpendicular) to the writing direction — that is, for a horizontal writing direction it’s vertical, and for a vertical writing direction, it’s horizontal. This attribute expresses the line position as a percentage of the dimensions of the video frame in the relevant direction. For example, 0 percent is the top of the video frame and 100 percent is the bottom of the video frame for horizontal writing layout.

If you use this attribute, apply it to the entire attributed string.

## See Also

### Layout

let kCMTextMarkupAttribute_VerticalLayout: CFString

The vertical layout of a text block.

let kCMTextMarkupAttribute_Alignment: CFString

The text alignment in the writing direction of the first line of text.

let kCMTextMarkupAttribute_TextPositionPercentageRelativeToWritingDirection: CFString

The placement of the block of text as a percentage in the writing direction.

let kCMTextMarkupAttribute_WritingDirectionSizePercentage: CFString

The width or height as a percentage of the bounding box that contains the text.

