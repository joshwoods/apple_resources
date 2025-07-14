

- Core Image
- CIImageProcessorOutput
-  baseAddress 

Instance Property

# baseAddress

A pointer to CPU memory at which to write output pixel data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var baseAddress: UnsafeMutableRawPointer { get }
```

**Required**

## Discussion

Use this property if you process the image using a CPU-based routine that cannot make use of higher-level constructs for sharing memory.

Note

If your image processing routine is GPU-based, use the the pixelBuffer, surface, or metalTexture property instead.

## See Also

### Providing Output Image Data

var metalTexture: (any MTLTexture)?

A Metal texture to which you can write output pixel data.

**Required**

var pixelBuffer: CVPixelBuffer?

A CoreVideo pixel buffer to which you can write output pixel data.

**Required**

var surface: IOSurfaceRef

An IOSurface object to which you can write output pixel data.

**Required**

