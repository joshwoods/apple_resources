

- Accelerate
- vImage_Buffer
-  init(width:height:bitsPerPixel:) 

Initializer

# init(width:height:bitsPerPixel:)

Creates a new buffer with the specified width, height, and bits per pixel.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init(
    width: Int,
    height: Int,
    bitsPerPixel: UInt32
) throws
```

## Parameters 

`width`  

The width of the buffer, in pixels.

`height`  

The height of the buffer, in pixels.

`bitsPerPixel`  

The number of bits in a single pixel.

## Mentioned in 

Creating and Populating Buffers from Core Graphics Images

## Discussion

This function allocates a buffer’s memory, but doesn’t initialize the memory.

## See Also

### Creating an empty vImage buffer

init(size: CGSize, bitsPerPixel: UInt32) throws

Creates a new buffer with the specified size and bits per pixel.

init()

Creates an empty vImage buffer.

