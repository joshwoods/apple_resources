

- Core Image
- CIImageProcessorInput
-  surface 

Instance Property

# surface

An IOSurface object containing the image data to be processed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var surface: IOSurfaceRef { get }
```

**Required**

## Discussion

Use this property if you plan to process the image using routines that can make use of memory shared with other processes or technologies.

Do not modify the contents of this surface.

## See Also

### Accessing Input Image Data

var baseAddress: UnsafeRawPointer

A pointer to the image data in CPU memory to be processed.

**Required**

var metalTexture: (any MTLTexture)?

A Metal texture containing the image data to be processed.

**Required**

var pixelBuffer: CVPixelBuffer?

A CoreVideo pixel buffer containing the image data to be processed.

**Required**

