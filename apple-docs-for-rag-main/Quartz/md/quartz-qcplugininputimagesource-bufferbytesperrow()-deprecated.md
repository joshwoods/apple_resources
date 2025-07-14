

- Quartz
- QCPlugInInputImageSource
-  bufferBytesPerRow() Deprecated

Instance Method

# bufferBytesPerRow()

Returns the bytes per row of the buffer representation.

macOS 10.4–10.15Deprecated

``` source
func bufferBytesPerRow() -> Int
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The number of bytes per row of the buffer.

## Discussion

The number of bytes per row is guaranteed to be a multiple of 16.

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

func bufferBaseAddress() -> UnsafeRawPointer!

Returns the base address of the image buffer.

**Required**

Deprecated

