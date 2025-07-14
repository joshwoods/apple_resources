

- Accelerate
- vImage
- vImage.PixelBuffer
-  copy(to:) 

Instance Method

# copy(to:)

Copies the contents of the pixel buffer to another pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func copy(to destinationBuffer: vImage.PixelBuffer)
```

Available when `Format` conforms to `StaticPixelFormat`.

## Parameters 

`destinationBuffer`  

The destination pixel buffer.

## See Also

### Pixel buffer methods

func copy(to: CVPixelBuffer, cvImageFormat: vImageCVImageFormat, cgImageFormat: vImage_CGImageFormat) throws

Copies the contents of a pixel buffer to a Core Video pixel buffer.

func makeCGImage(cgImageFormat: vImage_CGImageFormat) -> CGImage?

Returns a Core Graphics image from the pixel buffer’s contents.

func withCVPixelBuffer(readOnly: Bool, body: (CVPixelBuffer) -> Void)

Calls the given closure with a locked 32-bit BGRA Core Video Pixel Buffer.

