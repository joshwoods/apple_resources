

- Accelerate
- vImage
- vImage.PixelBuffer
-  init(planarBuffers:pixelFormat:) 

Initializer

# init(planarBuffers:pixelFormat:)

Returns an initialized buffer by copying the specified planar buffers.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    planarBuffers: [vImage.PixelBuffer],
    pixelFormat: Format.Type = Format.self
)
```

Available when `Format` conforms to `MultiplePlanePixelFormat`.

## Parameters 

`planarBuffers`  

An array that contains the source planar buffers.

`pixelFormat`  

The pixel format of the initialized buffer.

## Discussion

Note

The number of planar buffers must equal the `Format.planeCount`. All planar buffers must be the same size.

