

- Core Image
- CIImageProcessorOutput
-  surface 

Instance Property

# surface

An IOSurface object to which you can write output pixel data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var surface: IOSurfaceRef { get }
```

**Required**

## Discussion

Use this property if you plan to process the image using routines that can make use of memory shared with other processes or technologies.

## See Also

### Providing Output Image Data

var baseAddress: UnsafeMutableRawPointer

A pointer to CPU memory at which to write output pixel data.

**Required**

var metalTexture: (any MTLTexture)?

A Metal texture to which you can write output pixel data.

**Required**

var pixelBuffer: CVPixelBuffer?

A CoreVideo pixel buffer to which you can write output pixel data.

**Required**

