

- Accelerate
-  vImageCVImageFormat_Copy(\_:) 

Function

# vImageCVImageFormat_Copy(\_:)

Returns a mutable copy of an immutable Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_Copy(_ format: vImageConstCVImageFormat) -> Unmanaged!
```

## Parameters 

`format`  

The Core Video image format to copy.

## Return Value

A vImageCVImageFormat instance.

## Discussion

This function doesn’t copy the image format’s user data or the release callback.

