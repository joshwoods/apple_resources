

- AVFoundation
- AVVideoCompositionRenderContext
-  newPixelBuffer() 

Instance Method

# newPixelBuffer()

Returns a pixel buffer to use for rendering.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func newPixelBuffer() -> CVPixelBuffer?
```

## Return Value

A CVPixelBuffer to use for rendering.

## Discussion

The buffer’s kCVImageBufferCleanApertureKey and kCVImageBufferPixelAspectRatioKey attachments are set to match the current composition processor properties. You’re responsible for calling CVBufferRelease on the pixel buffer.

