

- MediaExtension
- MERAWProcessorPixelBufferManager
-  pixelBufferAttributes 

Instance Property

# pixelBufferAttributes

A dictionary that contains the attributes Video Toolbox uses to create a pixel buffer for the video RAW processor.

macOS 15.0+

``` source
var pixelBufferAttributes: [String : any Sendable] { get set }
```

## Discussion

The processor can update this dictionary before it requests a new pixel buffer.

## See Also

### Creating a pixel buffer

func makePixelBuffer() throws -> CVPixelBuffer

Generates a pixel buffer using the session’s pixel buffer pool.

