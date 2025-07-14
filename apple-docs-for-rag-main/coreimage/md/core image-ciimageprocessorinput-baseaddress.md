

- Core Image
- CIImageProcessorInput
-  baseAddress 

Instance Property

# baseAddress

A pointer to the image data in CPU memory to be processed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var baseAddress: UnsafeRawPointer { get }
```

**Required**

## Discussion

Use this property if you plan to process the image using a CPU-based routine that cannot make use of higher-level constructs for sharing memory.

Note

If your image processing routine is GPU-based, use the the pixelBuffer, surface, or metalTexture property instead.

Do not modify the memory addressed by this pointer.

## See Also

### Accessing Input Image Data

var metalTexture: (any MTLTexture)?

A Metal texture containing the image data to be processed.

**Required**

var pixelBuffer: CVPixelBuffer?

A CoreVideo pixel buffer containing the image data to be processed.

**Required**

var surface: IOSurfaceRef

An IOSurface object containing the image data to be processed.

**Required**

