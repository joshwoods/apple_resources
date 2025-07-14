

- Core Image
- CIImageProcessorInput
-  metalTexture 

Instance Property

# metalTexture

A Metal texture containing the image data to be processed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var metalTexture: (any MTLTexture)? { get }
```

**Required**

## Discussion

Use this property if you plan to process the image using a Metal shader.

Do not modify the contents of this texture.

## See Also

### Accessing Input Image Data

var baseAddress: UnsafeRawPointer

A pointer to the image data in CPU memory to be processed.

**Required**

var pixelBuffer: CVPixelBuffer?

A CoreVideo pixel buffer containing the image data to be processed.

**Required**

var surface: IOSurfaceRef

An IOSurface object containing the image data to be processed.

**Required**

