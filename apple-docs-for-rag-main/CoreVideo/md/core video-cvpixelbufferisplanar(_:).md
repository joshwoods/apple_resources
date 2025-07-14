

- Core Video
-  CVPixelBufferIsPlanar(\_:) 

Function

# CVPixelBufferIsPlanar(\_:)

Determines whether the pixel buffer is planar.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CVPixelBufferIsPlanar(_ pixelBuffer: CVPixelBuffer) -> Bool
```

## Parameters 

`pixelBuffer`  

The pixel buffer to check.

## Return Value

`true` if the pixel buffer is planar; otherwise, `false`.

## Discussion

Planar buffers can be created using the CVPixelBufferCreateWithPlanarBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) function.

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

func CVPixelBufferGetPlaneCount(CVPixelBuffer) -> Int

Returns number of planes of the pixel buffer.

func CVPixelBufferGetDataSize(CVPixelBuffer) -> Int

Returns the data size for contiguous planes of the pixel buffer.

func CVPixelBufferGetPixelFormatType(CVPixelBuffer) -> OSType

Returns the pixel format type of the pixel buffer.

func CVPixelBufferGetExtendedPixels(CVPixelBuffer, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;Int>?, UnsafeMutablePointer&lt;Int>?)

Returns the amount of extended pixel padding in the pixel buffer.

func CVPixelBufferGetIOSurface(CVPixelBuffer?) -> Unmanaged&lt;IOSurfaceRef>?

Returns the IOSurface backing the pixel buffer, or `NULL` if it is not backed by an IOSurface.

func CVPixelBufferCreateResolvedAttributesDictionary(CFAllocator?, CFArray?, UnsafeMutablePointer&lt;CFDictionary?>) -> CVReturn

Resolves an array of `CFDictionary` objects describing various pixel buffer attributes into a single dictionary.

func CVPixelBufferGetTypeID() -> CFTypeID

Returns the Core Foundation type identifier of the pixel buffer type.

