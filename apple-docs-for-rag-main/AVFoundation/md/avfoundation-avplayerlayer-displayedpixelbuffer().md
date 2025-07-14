

- AVFoundation
- AVPlayerLayer
-  displayedPixelBuffer() 

Instance Method

# displayedPixelBuffer()

Returns the pixel buffer that the player layer currently displays.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func displayedPixelBuffer() -> CVPixelBuffer?
```

## Return Value

The currently displayed pixel buffer, or `nil` if one isn’t available.

## Discussion

This method only returns an image when playback is in a paused state, and otherwise returns `nil`. It also returns `nil` when displaying protected content or if the layer isn’t currently displaying an image.

## See Also

### Processing Pixel Buffers

var pixelBufferAttributes: [String : Any]?

The attributes of the visual output that displays in the player layer during playback.

