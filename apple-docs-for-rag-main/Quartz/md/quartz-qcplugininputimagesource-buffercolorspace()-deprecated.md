

- Quartz
- QCPlugInInputImageSource
-  bufferColorSpace() Deprecated

Instance Method

# bufferColorSpace()

Returns the color space of the image buffer representation.

macOS 10.4–10.15Deprecated

``` source
func bufferColorSpace() -> Unmanaged!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

The color space of the image buffer.

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

func bufferBaseAddress() -> UnsafeRawPointer!

Returns the base address of the image buffer.

**Required**

Deprecated

func bufferBytesPerRow() -> Int

Returns the bytes per row of the buffer representation.

**Required**

Deprecated

