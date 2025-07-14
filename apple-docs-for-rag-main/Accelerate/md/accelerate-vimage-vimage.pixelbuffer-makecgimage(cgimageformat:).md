

- Accelerate
- vImage
- vImage.PixelBuffer
-  makeCGImage(cgImageFormat:) 

Instance Method

# makeCGImage(cgImageFormat:)

Returns a Core Graphics image from the pixel buffer’s contents.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func makeCGImage(cgImageFormat: vImage_CGImageFormat) -> CGImage?
```

Available when `Format` conforms to `StaticPixelFormat`.

## Parameters 

`cgImageFormat`  

The Core Graphics format of the source buffer.

## Return Value

A Core Graphics image that contains the source buffer’s contents.

## Mentioned in 

Converting bitmap data between Core Graphics images and vImage buffers

Optimizing image-processing performance

Applying flood fills to an image

## See Also

### Pixel buffer methods

func copy(to: vImage.PixelBuffer&lt;Format>)

Copies the contents of the pixel buffer to another pixel buffer.

func copy(to: CVPixelBuffer, cvImageFormat: vImageCVImageFormat, cgImageFormat: vImage_CGImageFormat) throws

Copies the contents of a pixel buffer to a Core Video pixel buffer.

func withCVPixelBuffer(readOnly: Bool, body: (CVPixelBuffer) -> Void)

Calls the given closure with a locked 32-bit BGRA Core Video Pixel Buffer.

