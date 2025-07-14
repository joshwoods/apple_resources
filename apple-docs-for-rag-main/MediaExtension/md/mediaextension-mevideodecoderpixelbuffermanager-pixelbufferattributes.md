

- MediaExtension
- MEVideoDecoderPixelBufferManager
-  pixelBufferAttributes 

Instance Property

# pixelBufferAttributes

A dictionary that contains the attributes Video Toolbox uses to create a pixel buffer for the decoder.

macOS 14.0+

``` source
var pixelBufferAttributes: [String : Any] { get set }
```

## Discussion

The decoder can update this dictionary before it requests a new pixel buffer.

## See Also

### Creating a pixel buffer

func makePixelBuffer() throws -> CVPixelBuffer

Generates a pixel buffer using the session’s pixel buffer pool.

