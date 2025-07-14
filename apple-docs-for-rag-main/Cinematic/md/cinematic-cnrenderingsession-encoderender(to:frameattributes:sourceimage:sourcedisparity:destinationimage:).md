

- Cinematic
- CNRenderingSession
-  encodeRender(to:frameAttributes:sourceImage:sourceDisparity:destinationImage:) 

Instance Method

# encodeRender(to:frameAttributes:sourceImage:sourceDisparity:destinationImage:)

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
func encodeRender(
    to commandBuffer: any MTLCommandBuffer,
    frameAttributes: CNRenderingSession.FrameAttributes,
    sourceImage: CVPixelBuffer,
    sourceDisparity: CVPixelBuffer,
    destinationImage: CVPixelBuffer
) -> Bool
```

