

- Quartz
- QCPlugInInputImageSource
-  bufferBaseAddress() Deprecated

Instance Method

# bufferBaseAddress()

Returns the base address of the image buffer.

macOS 10.4–10.15Deprecated

``` source
func bufferBaseAddress() -> UnsafeRawPointer!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The base address of the buffer.

## Discussion

The base address is guaranteed to be aligned on a 16-byte boundary.

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

func bufferPixelFormat() -> String!

Returns the pixel format of the image buffer representation.

**Required**

Deprecated

func bufferColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the image buffer representation.

**Required**

Deprecated

func bufferBytesPerRow() -> Int

Returns the bytes per row of the buffer representation.

**Required**

Deprecated

