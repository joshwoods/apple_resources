

- Accelerate
-  vImageCGImageFormat_IsEqual(\_:\_:) 

Function

# vImageCGImageFormat_IsEqual(\_:\_:)

Returns a Boolean value that indicates whether two vImage Core Graphics image formats are equal.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCGImageFormat_IsEqual(
    _ f1: UnsafePointer!,
    _ f2: UnsafePointer!
) -> Bool
```

## Parameters 

`f1`  

The first vImage_CGImageFormat structure. If colorSpace is `nil`, the function uses sRGB.

`f2`  

The second vImage_CGImageFormat structure. If colorSpace is `nil`, the function uses sRGB.

## Return Value

A Boolean value that indicates whether two vImage Core Graphics image formats are equal.

## See Also

### Querying Core Graphics image format attributes

func vImageCGImageFormat_GetComponentCount(UnsafePointer&lt;vImage_CGImageFormat>) -> UInt32

Calculates the number of color and alpha channels for a specified image format.

