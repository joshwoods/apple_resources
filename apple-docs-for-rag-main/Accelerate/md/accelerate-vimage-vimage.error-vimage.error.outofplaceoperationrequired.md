

- Accelerate
- vImage
- vImage.Error
-  vImage.Error.outOfPlaceOperationRequired 

Case

# vImage.Error.outOfPlaceOperationRequired

An error indicating that the source images and destination images alias the same image data, but must not.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case outOfPlaceOperationRequired
```

## See Also

### Enumeration Cases

case bufferSizeMismatch

An error indicating that the function requires the source and destination buffers to have the same size, but they don’t.

case colorSyncIsAbsent

An error indicating that the ColorSync framework is missing.

case coreVideoIsAbsent

An error indicating that the Core Video framework is missing.

case internalError

A serious error occurred inside vImage, which prevented vImage from continuing.

case invalidCVImageFormat

An error indicating that a Core Video format is invalid.

case invalidEdgeStyle

An error indicating that the specified edge style is invalid.

case invalidImageFormat

An error indicating that a specified Core Graphics or Core Video format is invalid.

case invalidImageObject

An error indicating that a specified Core Graphics image or Core Video pixel buffer is invalid.

case invalidKernelSize

An error indicating that either the kernel height, the kernel width, or both, are even.

case invalidOffset_X

An error indicating that the parameter that specifies the left edge of the region of interest is greater than the width of the source image.

case invalidOffset_Y

An error indicating that the parameter that specifies the top edge of the region of interest is greater than the height of the source image.

case invalidParameter

An error indicating that a function parameter has an invalid value.

case invalidRowBytes

An error indicating that the buffer’s row bytes field is invalid.

case memoryAllocationError

An error indicating that an attempt to allocate memory failed.

case noError

The vImage function completed without error.

