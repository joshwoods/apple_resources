

- Image I/O
-  CGImageSourceGetPrimaryImageIndex(\_:) 

Function

# CGImageSourceGetPrimaryImageIndex(\_:)

Returns the index of the primary image for an High Efficiency Image File Format (HEIF) image.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func CGImageSourceGetPrimaryImageIndex(_ isrc: CGImageSource) -> Int
```

## Parameters 

`isrc`  

The image source that contains the image data.

## Return Value

The index of the primary image, or `0` for image formats other than the HEIF format.

## See Also

### Extracting Images From an Image Source

func CGImageSourceCreateImageAtIndex(CGImageSource, Int, CFDictionary?) -> CGImage?

Creates an image object from the data at the specified index in an image source.

func CGImageSourceCreateThumbnailAtIndex(CGImageSource, Int, CFDictionary?) -> CGImage?

Creates a thumbnail version of the image at the specified index in an image source.

