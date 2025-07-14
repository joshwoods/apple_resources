

- Accelerate
- vImage_Buffer
-  init(data:height:width:rowBytes:) 

Initializer

# init(data:height:width:rowBytes:)

Creates a new buffer with the specified size that references existing data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    data: UnsafeMutableRawPointer!,
    height: vImagePixelCount,
    width: vImagePixelCount,
    rowBytes: Int
)
```

## Parameters 

`data`  

A pointer to the top-left pixel of the buffer.

`height`  

The height of the buffer, in pixels.

`width`  

The width of the buffer, in pixels.

`rowBytes`  

The number of bytes in a pixel row.

## Discussion

If you provide your own buffer storage, call preferredAlignmentAndRowBytes(width:height:bitsPerPixel:) to get the row stride that ensures your buffer achieves the best performance.

```
let width = 10
let height = 5

let alignmentAndRowBytes = try vImage_Buffer.preferredAlignmentAndRowBytes(
    width: width,
    height: height,
    bitsPerPixel: 8)

// Prints "16".
print(alignmentAndRowBytes.rowBytes)

let data = UnsafeMutableRawPointer.allocate(
    byteCount: alignmentAndRowBytes.rowBytes * height,
    alignment: alignmentAndRowBytes.alignment)

let buffer = vImage_Buffer(data: data,
                           height: vImagePixelCount(height),
                           width: vImagePixelCount(width),
                           rowBytes: alignmentAndRowBytes.rowBytes)
```

## See Also

### Creating a buffer that references existing data

static func preferredAlignmentAndRowBytes(width: Int, height: Int, bitsPerPixel: UInt32) throws -> (alignment: Int, rowBytes: Int)

Returns the preferred alignment and row bytes for a specified size and bits per pixel.

