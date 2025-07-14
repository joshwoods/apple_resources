

- Accelerate
- vImage
- vImage.EdgeMode
-  vImage.EdgeMode.truncateKernel 

Case

# vImage.EdgeMode.truncateKernel

An edge mode that uses only the part of the kernel that overlaps the image.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
case truncateKernel
```

## See Also

### Enumeration Cases

case copyInPlace

An edge mode that copies the value of the edge pixel in the source to the destination.

case extend

An edge mode that extends the edges of the image infinitely.

case fill(backgroundColor: PixelType)

An edge mode that uses the background color for missing pixels.

