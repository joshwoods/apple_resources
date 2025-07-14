

- Accelerate
-  kvImageCopyInPlace 

Global Variable

# kvImageCopyInPlace

A flag that copies the value of the edge pixel in the source to the destination.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var kvImageCopyInPlace: Int { get }
```

## Discussion

When you set this flag, and a convolution function is processing an image pixel for which some of the kernel extends beyond the image boundaries, vImage does not compute the convolution. Instead, the value of the particular pixel unchanged; it’s simply copied to the destination image. This flag is valid only for convolution operations. The morphology functions do not use this flag because they do not use pixels outside the image in any of their calculations.

## See Also

### Edging Modes

var kvImageBackgroundColorFill: Int

A flag that uses the background color for missing pixels.

var kvImageEdgeExtend: Int

A flag that extends the edges of the image infinitely.

var kvImageTruncateKernel: Int

A flag that uses only the part of the kernel that overlaps the image.

