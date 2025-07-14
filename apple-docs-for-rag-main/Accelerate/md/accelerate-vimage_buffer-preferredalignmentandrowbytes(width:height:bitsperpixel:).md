

- Accelerate
- vImage_Buffer
-  preferredAlignmentAndRowBytes(width:height:bitsPerPixel:) 

Type Method

# preferredAlignmentAndRowBytes(width:height:bitsPerPixel:)

Returns the preferred alignment and row bytes for a specified size and bits per pixel.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func preferredAlignmentAndRowBytes(
    width: Int,
    height: Int,
    bitsPerPixel: UInt32
) throws -> (alignment: Int, rowBytes: Int)
```

## Parameters 

`width`  

The width of the image, in pixels.

`height`  

The height of the image, in pixels.

`bitsPerPixel`  

The number of bits in a single pixel.

## Return Value

A tuple that contains the alignment and row bytes.

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

init(data: UnsafeMutableRawPointer!, height: vImagePixelCount, width: vImagePixelCount, rowBytes: Int)

Creates a new buffer with the specified size that references existing data.

