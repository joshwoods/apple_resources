

- Accelerate
- vImage
- vImage.PixelBuffer
-  overwriteChannels(withScalar:) 

Instance Method

# overwriteChannels(withScalar:)

Overwrites the pixels of the pixel buffer with the provided 32-bit scalar value.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func overwriteChannels(withScalar scalar: Pixel_F)
```

Available when `Format` is `vImage.PlanarF`.

## Parameters 

`scalar`  

The value that the function writes to the channels.

## See Also

### Overwriting Channels

func overwriteChannels(withScalar: Pixel_8)

Overwrites the pixels of the pixel buffer with the provided 8-bit scalar value.

func overwriteChannels(withScalar: Pixel_16F)

Overwrites the pixels of the pixel buffer with the provided floating-point 16-bit scalar value.

func overwriteChannels([UInt8], withScalar: Pixel_8, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit scalar value.

func overwriteChannels([UInt8], withScalar: Pixel_F, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit scalar value.

func overwriteChannels([UInt8], withPixel: Pixel_8888, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit, 4-channel pixel value.

func overwriteChannels([UInt8], withPixel: Pixel_ARGB_16U, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided unsigned 16-bit, 4-channel pixel value.

func overwriteChannels([UInt8], withPixel: Pixel_FFFF, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit, 4-channel pixel value.

func overwriteChannels([UInt8], withPlanarBuffer: vImage.PixelBuffer&lt;vImage.Planar8>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit planar pixel buffer.

func overwriteChannels([UInt8], withPlanarBuffer: vImage.PixelBuffer&lt;vImage.PlanarF>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit planar pixel buffer.

func overwriteChannels([UInt8], withInterleavedBuffer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit interleaved pixel buffer.

func overwriteChannels([UInt8], withInterleavedBuffer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit interleaved pixel buffer.

