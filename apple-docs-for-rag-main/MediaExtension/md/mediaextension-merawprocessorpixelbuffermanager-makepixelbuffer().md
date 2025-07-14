

- MediaExtension
- MERAWProcessorPixelBufferManager
-  makePixelBuffer() 

Instance Method

# makePixelBuffer()

Generates a pixel buffer using the session’s pixel buffer pool.

macOS 15.0+

``` source
func makePixelBuffer() throws -> CVPixelBuffer
```

## Return Value

A pixel buffer that’s compatible with the extension’s most recently set pixel buffer attributes.

## See Also

### Creating a pixel buffer

var pixelBufferAttributes: [String : any Sendable]

A dictionary that contains the attributes Video Toolbox uses to create a pixel buffer for the video RAW processor.

