

- Core Media
-  kCMTextMarkupAlignmentType_Left 

Global Variable

# kCMTextMarkupAlignmentType_Left

An alignment type that visually aligns text from left-to-right.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
let kCMTextMarkupAlignmentType_Left: CFString
```

## Discussion

For horizontally written text, the text alignment is always visually left-aligned (the system uniformly treats left-to-right and right-to-left). For vertical text, kCMTextMarkupAlignmentType_Left is equivalent to kCMTextMarkupAlignmentType_Start.

## See Also

### Alignment Types

let kCMTextMarkupAlignmentType_Start: CFString

An alignment type that visually aligns the text at its starting side.

let kCMTextMarkupAlignmentType_Middle: CFString

An alignment type that visually aligns text in the center between its starting and ending sides.

let kCMTextMarkupAlignmentType_End: CFString

An alignment type that visually aligns the text at its ending side.

let kCMTextMarkupAlignmentType_Right: CFString

An alignment type that visually aligns text from right-to-left.

