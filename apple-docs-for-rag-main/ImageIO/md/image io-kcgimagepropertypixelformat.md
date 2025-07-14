

- Image I/O
-  kCGImagePropertyPixelFormat 

Global Variable

# kCGImagePropertyPixelFormat

The format of the image’s individual pixels.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
let kCGImagePropertyPixelFormat: CFString
```

## Discussion

The value of this property is a CFNumber. For information about how to interpret this value, see the `PixelFormat` tag in the EXIF specification.

## See Also

### Pixel Information

let kCGImagePropertyPixelWidth: CFString

The number of pixels along the x-axis of the image.

let kCGImagePropertyPixelHeight: CFString

The number of pixels along the y-axis of the image.

let kCGImagePropertyDPIHeight: CFString

The resolution, in dots per inch, in the y dimension.

let kCGImagePropertyDPIWidth: CFString

The resolution, in dots per inch, in the x dimension.

let kCGImagePropertyDepth: CFString

The number of bits in the color sample of a pixel.

