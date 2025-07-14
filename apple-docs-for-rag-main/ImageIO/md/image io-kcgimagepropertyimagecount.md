

- Image I/O
-  kCGImagePropertyImageCount 

Global Variable

# kCGImagePropertyImageCount

The number of images in the file.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCGImagePropertyImageCount: CFString
```

## Discussion

The value of this property is a CFNumber.

## See Also

### Image Information

let kCGImagePropertyIsIndexed: CFString

A Boolean value that indicates whether the image contains indexed pixel samples.

let kCGImagePropertyImages: CFString

An array of dictionaries, each of which contains metadata for one of the images in the file.

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

