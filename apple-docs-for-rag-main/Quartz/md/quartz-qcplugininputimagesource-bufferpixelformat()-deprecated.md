

- Quartz
- QCPlugInInputImageSource
-  bufferPixelFormat() Deprecated

Instance Method

# bufferPixelFormat()

Returns the pixel format of the image buffer representation.

macOS 10.4–10.15Deprecated

``` source
func bufferPixelFormat() -> String!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A string that specifies the pixel format. The supported formats are ARGB8 (8-bit alpha, red, green, blue), BGRA8 (8-bit blue, green, red, and alpha), RGBAf (floating-point, red, green, blue, alpha), I8 (8-bit intensity), and If (floating-point intensity).

## See Also

### Getting Image Buffer Information

func imageBounds() -> NSRect

Returns the actual bounds of the image source expressed in pixels and aligned to integer boundaries.

**Required**

Deprecated

func bufferPixelsWide() -> Int

Returns the width of the image buffer representation.

**Required**

Deprecated

func bufferPixelsHigh() -> Int

Returns the height of the image buffer representation.

**Required**

Deprecated

func bufferColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the image buffer representation.

**Required**

Deprecated

func bufferBaseAddress() -> UnsafeRawPointer!

Returns the base address of the image buffer.

**Required**

Deprecated

func bufferBytesPerRow() -> Int

Returns the bytes per row of the buffer representation.

**Required**

Deprecated

