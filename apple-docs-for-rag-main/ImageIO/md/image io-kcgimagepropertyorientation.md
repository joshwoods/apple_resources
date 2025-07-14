

- Image I/O
-  kCGImagePropertyOrientation 

Global Variable

# kCGImagePropertyOrientation

The intended display orientation of the image.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyOrientation: CFString
```

## Discussion

The value of this property is a CFNumber. The value encodes the intended display orientation for the image according to the TIFF and EXIF specifications. See the CGImagePropertyOrientation type for possible values and their meanings.

## See Also

### Image Information

let kCGImagePropertyImageCount: CFString

The number of images in the file.

let kCGImagePropertyIsIndexed: CFString

A Boolean value that indicates whether the image contains indexed pixel samples.

let kCGImagePropertyImages: CFString

An array of dictionaries, each of which contains metadata for one of the images in the file.

let kCGImagePropertyThumbnailImages: CFString

let kCGImagePropertyPrimaryImage: CFString

The index of the primary image in the file.

let kCGImagePropertyIsFloat: CFString

A Boolean value that indicates whether the image contains floating-point pixel samples.

Individual Image Properties

Properties that apply to an individual image in an image source.

enum CGImagePropertyOrientation

A value describing the intended display orientation for an image.

