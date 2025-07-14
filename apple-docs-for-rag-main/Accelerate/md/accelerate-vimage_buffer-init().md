

- Accelerate
- vImage_Buffer
-  init() 

Initializer

# init()

Creates an empty vImage buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init()
```

## Discussion

Use this initializer to create an empty vImage buffer that you pass to a subsequent function that allocates and initializes the buffer’s storage and properties. For example, the following code creates an empty buffer and initializes it using the vImageBuffer_Init(_:_:_:_:_:) function:

```
var buffer = vImage_Buffer()

vImageBuffer_Init(&buffer,
                  5,    // height
                  10,   // width
                  8,    // bits per pixel
                  vImage_Flags(kvImageNoFlags))

```

## See Also

### Creating an empty vImage buffer

init(width: Int, height: Int, bitsPerPixel: UInt32) throws

Creates a new buffer with the specified width, height, and bits per pixel.

init(size: CGSize, bitsPerPixel: UInt32) throws

Creates a new buffer with the specified size and bits per pixel.

