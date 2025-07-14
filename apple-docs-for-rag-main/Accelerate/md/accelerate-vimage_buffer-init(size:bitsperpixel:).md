

- Accelerate
- vImage_Buffer
-  init(size:bitsPerPixel:) 

Initializer

# init(size:bitsPerPixel:)

Creates a new buffer with the specified size and bits per pixel.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
init(
    size: CGSize,
    bitsPerPixel: UInt32
) throws
```

## Parameters 

`size`  

The size of the buffer, in pixels.

`bitsPerPixel`  

The number of bits in a single pixel.

## Discussion

This function allocates a buffer’s memory, but doesn’t initialize the memory.

## See Also

### Creating an empty vImage buffer

init(width: Int, height: Int, bitsPerPixel: UInt32) throws

Creates a new buffer with the specified width, height, and bits per pixel.

init()

Creates an empty vImage buffer.

