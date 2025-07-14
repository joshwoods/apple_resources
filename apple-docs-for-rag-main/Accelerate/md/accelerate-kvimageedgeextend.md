

- Accelerate
-  kvImageEdgeExtend 

Global Variable

# kvImageEdgeExtend

A flag that extends the edges of the image infinitely.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var kvImageEdgeExtend: Int { get }
```

## Discussion

When you set this flag, vImage replicates the edges of the image outward. It repeats the top row of the image infinitely above the image, the bottom row infinitely below the image, the first column infinitely to the left of the image, and the last column infinitely to the right. For spaces that are diagonal to the image, vImage uses the value of the corresponding corner pixel.

For example, for all pixels that are both above and to the left of the image, the upper-leftmost pixel of the image (the pixel at row 0, column 0) supplies the value. In this way, vImage assigns every pixel location outside the image some value. You can set this flag for convolution and geometry functions. The morphology functions do not use this flag because they do not use pixels outside the image in any of their calculations.

## See Also

### Edging Modes

var kvImageCopyInPlace: Int

A flag that copies the value of the edge pixel in the source to the destination.

var kvImageBackgroundColorFill: Int

A flag that uses the background color for missing pixels.

var kvImageTruncateKernel: Int

A flag that uses only the part of the kernel that overlaps the image.

