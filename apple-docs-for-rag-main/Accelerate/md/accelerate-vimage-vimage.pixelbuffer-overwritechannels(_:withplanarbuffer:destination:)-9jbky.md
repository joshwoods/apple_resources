

- Accelerate
- vImage
- vImage.PixelBuffer
-  overwriteChannels(\_:withPlanarBuffer:destination:) 

Instance Method

# overwriteChannels(\_:withPlanarBuffer:destination:)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit planar pixel buffer.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func overwriteChannels(
    _ channels: [UInt8],
    withPlanarBuffer buffer: vImage.PixelBuffer,
    destination: vImage.PixelBuffer
)
```

Available when `Format` is `vImage.Interleaved8x4`.

## Parameters 

`channels`  

An array that contains the indices of the channels that the function overwrites.

`buffer`  

The planar buffer that the function writes to the channels.

`destination`  

The destination pixel buffer.

## Discussion

Use this function to overwrite one or more channels of an interleaved buffer with a planar buffer. The following code overwrites channels `1` and `3` with the values in `overwriteValues`:

```
let pixelValues: [Pixel_8] = [ 1, 2, 3, 4,
                               5, 6, 7, 8 ]
let buffer = vImage.PixelBuffer(pixelValues: pixelValues,
                                size: vImage.Size(width: 1,
                                                  height: 2),
                                pixelFormat: vImage.Interleaved8x4.self)

let destination = vImage.PixelBuffer(size: vImage.Size(width: 1,
                                                       height: 2),
                                     pixelFormat: vImage.Interleaved8x4.self)

let overwriteValues: [Pixel_8] = [ 101,
                                   102 ]

let overwriteBuffer = vImage.PixelBuffer(pixelValues: overwriteValues,
                                                         size: vImage.Size(width: 1,
                                                                           height: 2))

buffer.overwriteChannels([3, 1],
                         withPlanarBuffer: overwriteBuffer,
                         destination: destination)
```

On return, `destination.array` contains the following values:

```
[ 1, 101, 3, 101,
  5, 102, 7, 102 ]
```

## See Also

### Overwriting Channels

func overwriteChannels(withScalar: Pixel_8)

Overwrites the pixels of the pixel buffer with the provided 8-bit scalar value.

func overwriteChannels(withScalar: Pixel_16F)

Overwrites the pixels of the pixel buffer with the provided floating-point 16-bit scalar value.

func overwriteChannels(withScalar: Pixel_F)

Overwrites the pixels of the pixel buffer with the provided 32-bit scalar value.

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

func overwriteChannels([UInt8], withPlanarBuffer: vImage.PixelBuffer&lt;vImage.PlanarF>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit planar pixel buffer.

func overwriteChannels([UInt8], withInterleavedBuffer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 8-bit interleaved pixel buffer.

func overwriteChannels([UInt8], withInterleavedBuffer: vImage.PixelBuffer&lt;Format>, destination: vImage.PixelBuffer&lt;Format>)

Overwrites the pixels of one or more channels of the pixel buffer with the provided 32-bit interleaved pixel buffer.

