

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(data:width:height:byteCountPerRow:pixelFormat:) 

Initializer

# init(data:width:height:byteCountPerRow:pixelFormat:)

Returns a new buffer that references existing data.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    data: UnsafeMutableRawPointer,
    width: Int,
    height: Int,
    byteCountPerRow: Int,
    pixelFormat: Format.Type
)
```

Available when `Format` conforms to `SinglePlanePixelFormat`.

## Parameters 

`data`  

A pointer to the top-left pixel of the buffer.

`width`  

The width, in pixels, of the pixel buffer.

`height`  

The height, in pixels, of the pixel buffer.

`byteCountPerRow`  

The number of bytes in a pixel row.

`pixelFormat`  

The pixel format of the initialized buffer.

## Discussion

You can use this function to simplify interoperation with other libraries and frameworks. For example, the following code shows a function that permutes the channels of a CGImage instance. The function creates a pixel buffer that uses the storage a CGDataProvider instance’s data property provides. The data property is a copy of the image data, therefore, the code returns a new CGImage instance that it generates from the permuted pixel buffer.

```
static func permute(image: CGImage,
                    to permuteMap: (UInt8, UInt8, UInt8, UInt8)) -> CGImage? {

    let bitsPerPixel = image.bitsPerPixel
    let bitsPerComponent = image.bitsPerComponent

    guard bitsPerPixel == 32 && bitsPerComponent == 8,
          let format = vImage_CGImageFormat(cgImage: image),
          let pixelData = image.dataProvider?.data else {
        return nil
    }

    return withExtendedLifetime(pixelData) {
        let pixelBuffer = vImage.PixelBuffer(
            data: UnsafeMutableRawPointer(mutating: CFDataGetBytePtr($0)),
            width: image.width,
            height: image.height,
            byteCountPerRow: image.bytesPerRow,
            pixelFormat: vImage.Interleaved8x4.self)

        pixelBuffer.permuteChannels(to: permuteMap,
                                    destination: pixelBuffer)

        return pixelBuffer.makeCGImage(cgImageFormat: format)
    }
}
```

Important

The pixel buffer is valid only for the lifetime of `data`.

## See Also

### Creating a pixel buffer from raw pixel data

init&lt;U>(pixelValues: U, size: vImage.Size, pixelFormat: Format.Type)

Creates a new pixel buffer by copying the supplied collection of pixel values.

init(data: UnsafeMutableRawPointer, width: Int, height: Int, byteCountPerRow: Int?, pixelFormat: Format.Type)

Calculates the correct bytes per row and returns a new buffer that references existing data.

