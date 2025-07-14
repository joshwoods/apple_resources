

- Accelerate
-  vImageCGImageFormat_GetComponentCount(\_:) 

Function

# vImageCGImageFormat_GetComponentCount(\_:)

Calculates the number of color and alpha channels for a specified image format.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCGImageFormat_GetComponentCount(_ format: UnsafePointer) -> UInt32
```

## Parameters 

`format`  

A valid vImage_CGImageFormat structure.

## Return Value

The number of color and alpha channels in the image.

## See Also

### Querying Core Graphics image format attributes

func vImageCGImageFormat_IsEqual(UnsafePointer&lt;vImage_CGImageFormat>!, UnsafePointer&lt;vImage_CGImageFormat>!) -> Bool

Returns a Boolean value that indicates whether two vImage Core Graphics image formats are equal.

