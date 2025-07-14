

- Accelerate
-  vImagePNGDecompressionFilter(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImagePNGDecompressionFilter(\_:\_:\_:\_:\_:\_:\_:)

Performs PNG decompression filtering.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImagePNGDecompressionFilter(
    _ buffer: UnsafePointer!,
    _ startScanline: vImagePixelCount,
    _ scanlineCount: vImagePixelCount,
    _ bitsPerPixel: UInt32,
    _ filterMethodNumber: UInt32,
    _ filterType: UInt32,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`buffer`  

On input, the image data to filter. On output, the filtered data. The filtering is always applied in place.

`startScanline`  

The starting scanline.

`scanlineCount`  

The number of scanlines in the buffer.

`bitsPerPixel`  

The bits per pixel.

`filterMethodNumber`  

The filter method number. You must pass `0`, because this is the only filtering method offered by this function.

`filterType`  

The filtering algorithm to apply to the image data. For filter method `0`, you can pass any of the constants described in PNG Filter Types.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile.

## Return Value

kvImageNoError; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

This function implements PNG decompression filtering for filter method `0` of the PNG standard, section 9.2, as described in: http://www.w3.org/TR/PNG-Filters.html. When a pixel that is needed for a filtering calculation falls outside the source buffer, its value is presumed to be `0`.

