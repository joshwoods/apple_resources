

- Core Media
-  kCMTextMarkupAttribute_Alignment 

Global Variable

# kCMTextMarkupAttribute_Alignment

The text alignment in the writing direction of the first line of text.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAttribute_Alignment: CFString
```

## Discussion

This attribute’s value must be one of the constants listed below that indicate the alignment in the writing direction of the first line of text of the cue. The value (or absence) of the kCMTextMarkupAttribute_VerticalLayout attribute indicates the writing direction. The default value of this attribute is kCMTextMarkupAlignmentType_Middle.

If you use this attribute, apply it to the entire attributed string.

## Topics

### Alignment Types

let kCMTextMarkupAlignmentType_Start: CFString

An alignment type that visually aligns the text at its starting side.

let kCMTextMarkupAlignmentType_Middle: CFString

An alignment type that visually aligns text in the center between its starting and ending sides.

let kCMTextMarkupAlignmentType_End: CFString

An alignment type that visually aligns the text at its ending side.

let kCMTextMarkupAlignmentType_Left: CFString

An alignment type that visually aligns text from left-to-right.

let kCMTextMarkupAlignmentType_Right: CFString

An alignment type that visually aligns text from right-to-left.

## See Also

### Layout

let kCMTextMarkupAttribute_VerticalLayout: CFString

The vertical layout of a text block.

let kCMTextMarkupAttribute_TextPositionPercentageRelativeToWritingDirection: CFString

The placement of the block of text as a percentage in the writing direction.

let kCMTextMarkupAttribute_OrthogonalLinePositionPercentageRelativeToWritingDirection: CFString

The placement of the first line in a block of text as a percentage in the direction orthogonal to the writing direction.

let kCMTextMarkupAttribute_WritingDirectionSizePercentage: CFString

The width or height as a percentage of the bounding box that contains the text.

