

- Core Video
-  CVPixelBufferGetIOSurface(\_:) 

Function

# CVPixelBufferGetIOSurface(\_:)

Returns the IOSurface backing the pixel buffer, or `NULL` if it is not backed by an IOSurface.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func CVPixelBufferGetIOSurface(_ pixelBuffer: CVPixelBuffer?) -> Unmanaged?
```

## See Also

### Inspecting Pixel Buffers

func CVPixelBufferGetBaseAddress(CVPixelBuffer) -> UnsafeMutableRawPointer?

Returns the base address of the pixel buffer.

func CVPixelBufferGetBaseAddressOfPlane(CVPixelBuffer, Int) -> UnsafeMutableRawPointer?

Returns the base address of the plane at the specified plane index.

func CVPixelBufferGetBytesPerRow(CVPixelBuffer) -> Int

Returns the number of bytes per row of the pixel buffer.

func CVPixelBufferGetBytesPerRowOfPlane(CVPixelBuffer, Int) -> Int

Returns the number of bytes per row for a plane at the specified index in the pixel buffer.

func CVPixelBufferGetHeight(CVPixelBuffer) -> Int

Returns the height of the pixel buffer.

func CVPixelBufferGetHeightOfPlane(CVPixelBuffer, Int) -> Int

Returns the height of the plane at planeIndex in the pixel buffer.

func CVPixelBufferGetWidth(CVPixelBuffer) -> Int

Returns the width of the pixel buffer.

func CVPixelBufferGetWidthOfPlane(CVPixelBuffer, Int) -> Int

Returns the width of the plane at a given index in the pixel buffer.

func CVPixelBufferIsPlanar(CVPixelBuffer) -> Bool

Determines whether the pixel buffer is planar.

func CVPixelBufferGetPlaneCount(CVPixelBuffer) -> Int

Returns number of planes of the pixel buffer.

func CVPixelBufferGetDataSize(CVPixelBuffer) -> Int

Returns the data size for contiguous planes of the pixel buffer.

func CVPixelBufferGetPixelFormatType(CVPixelBuffer) -> OSType

Returns the pixel format type of the pixel buffer.

func CVPixelBufferGetExtendedPixels(CVPixelBuffer, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;Int>?)

Returns the amount of extended pixel padding in the pixel buffer.

func CVPixelBufferCreateResolvedAttributesDictionary(CFAllocator?, CFArray?, UnsafeMutablePointer&lt;CFDictionary?>) -> CVReturn

Resolves an array of `CFDictionary` objects describing various pixel buffer attributes into a single dictionary.

func CVPixelBufferGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the pixel buffer type.

