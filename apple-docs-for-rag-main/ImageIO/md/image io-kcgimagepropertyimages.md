

- Image I/O
-  kCGImagePropertyImages 

Global Variable

# kCGImagePropertyImages

An array of dictionaries, each of which contains metadata for one of the images in the file.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCGImagePropertyImages: CFString
```

## Discussion

The value of this property is a CFArray. Each element in the array is a CFDictionary that contains metadata for one of the images. For example, the dictionary might contain the width and height of the image, the image’s color space name, thumbnail image information, and any auxiliary data.

## See Also

### Image Information

let kCGImagePropertyImageCount: CFString

The number of images in the file.

let kCGImagePropertyIsIndexed: CFString

A Boolean value that indicates whether the image contains indexed pixel samples.

let kCGImagePropertyThumbnailImages: CFString

let kCGImagePropertyPrimaryImage: CFString

The index of the primary image in the file.

let kCGImagePropertyIsFloat: CFString

A Boolean value that indicates whether the image contains floating-point pixel samples.

let kCGImagePropertyOrientation: CFString

The intended display orientation of the image.

Individual Image Properties

Properties that apply to an individual image in an image source.

enum CGImagePropertyOrientation

A value describing the intended display orientation for an image.

