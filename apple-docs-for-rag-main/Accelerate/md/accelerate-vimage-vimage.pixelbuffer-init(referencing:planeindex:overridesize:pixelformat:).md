

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(referencing:planeIndex:overrideSize:pixelFormat:) 

Initializer

# init(referencing:planeIndex:overrideSize:pixelFormat:)

Initializes a pixel buffer by refencing the data from a single plane of a multiplane Core Video pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    referencing lockedCVPixelBuffer: CVPixelBuffer,
    planeIndex: Int,
    overrideSize: vImage.Size? = nil,
    pixelFormat: Format.Type = Format.self
)
```

Available when `Format` conforms to `SinglePlanePixelFormat`.

## Parameters 

`lockedCVPixelBuffer`  

The locked Core Video pixel buffer. Use CVPixelBufferLockBaseAddress(_:_:) and CVPixelBufferUnlockBaseAddress(_:_:) to lock and unlock the pixel buffer.

`planeIndex`  

The index of the plane that the function references.

`overrideSize`  

An optional size that overrides the size returned by CVPixelBufferGetHeightOfPlane(_:_:) and CVPixelBufferGetWidthOfPlane(_:_:). Use this parameter if you intend to pass the buffer to the any-to-any converter that requires all buffers to be the same size.

`pixelFormat`  

The pixel format of the initialized buffer.

## See Also

### Creating a pixel buffer from a Core Video buffer

init(copying: CVPixelBuffer, cvImageFormat: vImageCVImageFormat, cgImageFormat: inout vImage_CGImageFormat, pixelFormat: Format.Type) throws

Initializes a pixel buffer by copying the data from a Core Video pixel buffer.

init(referencing: CVPixelBuffer, converter: vImageConverter, destinationPixelFormat: Format.Type)

Returns a new pixel buffer that references the specified Core Video pixel buffer and populated converter.

