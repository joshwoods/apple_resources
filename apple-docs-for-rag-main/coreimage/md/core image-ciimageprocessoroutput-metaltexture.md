

- Core Image
- CIImageProcessorOutput
-  metalTexture 

Instance Property

# metalTexture

A Metal texture to which you can write output pixel data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var metalTexture: (any MTLTexture)? { get }
```

**Required**

## Discussion

For image processing using a Metal shader, bind this texture as an attachment in a render pass or as an output texture in a compute pass.

## See Also

### Providing Output Image Data

var baseAddress: UnsafeMutableRawPointer

A pointer to CPU memory at which to write output pixel data.

**Required**

var pixelBuffer: CVPixelBuffer?

A CoreVideo pixel buffer to which you can write output pixel data.

**Required**

var surface: IOSurfaceRef

An IOSurface object to which you can write output pixel data.

**Required**

