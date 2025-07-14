

- AVFoundation
- AVPlayerLayer
-  pixelBufferAttributes 

Instance Property

# pixelBufferAttributes

The attributes of the visual output that displays in the player layer during playback.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var pixelBufferAttributes: [String : Any]? { get set }
```

## Discussion

Use this property to customize the format of the pixel buffers that the player layer vends.

## See Also

### Processing Pixel Buffers

func displayedPixelBuffer() -> CVPixelBuffer?

Returns the pixel buffer that the player layer currently displays.

