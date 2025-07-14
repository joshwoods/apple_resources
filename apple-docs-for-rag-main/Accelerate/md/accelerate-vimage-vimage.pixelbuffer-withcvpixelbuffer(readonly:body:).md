

- Accelerate
- vImage
- vImage.PixelBuffer
-  withCVPixelBuffer(readOnly:body:) 

Instance Method

# withCVPixelBuffer(readOnly:body:)

Calls the given closure with a locked 32-bit BGRA Core Video Pixel Buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func withCVPixelBuffer(
    readOnly: Bool,
    body: (CVPixelBuffer) -> Void
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`readOnly`  

A Boolean value that specifies whether the function locks the CVPixelBuffer with the readOnly flag. If the closure doesn’t modify the data, set this parameter to `true`.

`body`  

A closure with a CVPixelBuffer parameter that points to the underlying pixel buffer image data.

## Discussion

Use this function to pass a vImage pixel buffer to other frameworks. For example, the following code creates a Core Image CIImage instance from a CVPixelBuffer that shares its underlying storage with a pixel buffer:

```
let src = vImage.PixelBuffer(
    size: vImage.Size(width: 64, height: 64))

src.withCVPixelBuffer(readOnly: false) { cvPixelBuffer in

    let ciImage = CIImage(cvImageBuffer: cvPixelBuffer)

    // Core Image workflow using `ciImage`
}
```

## See Also

### Pixel buffer methods

func copy(to: vImage.PixelBuffer&lt;Format>)

Copies the contents of the pixel buffer to another pixel buffer.

func copy(to: CVPixelBuffer, cvImageFormat: vImageCVImageFormat, cgImageFormat: vImage_CGImageFormat) throws

Copies the contents of a pixel buffer to a Core Video pixel buffer.

func makeCGImage(cgImageFormat: vImage_CGImageFormat) -> CGImage?

Returns a Core Graphics image from the pixel buffer’s contents.

